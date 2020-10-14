---
title:  Membuat factory reset dinamis
tags:
  - Btrfs
  - Linux
  - Snapper
  - Snapshot
  - Tips & Trik
  - openSUSE
---

Ada kekurangan dari [fitur factory reset]({{site.baseurl}}/2020/09/03/membuat-fitur-factory-reset.html), yaitu ketika kita sudah menggunakan komputer dalam jangka waktu yang sangat lama, berbulan-bulan atau bahkan bertahun-tahun, lalu kita lakukan *factory reset*, maka sistem operasi kita akan kembali ke masa lalu. Contohnya jika kita mengatur *factory reset* setelah instalasi openSUSE Leap 15.2, lalu setahun kemudian kita melakukan *upgrade* ke openSUSE Leap 15.3, lalu tahun berikutnya kita *upgrade* lagi ke openSUSE Leap berikutnya. Jika kemudian kita melakukan *factory reset*, maka komputer kita akan kembali ke openSUSE Leap 15.2. Dan jika setelahnya kita lakukan *upgrade* lagi ke openSUSE Leap terbaru di saat itu mungkin akan terjadi masalah karena peningkatan versi yang terlalu jauh.

<!--more-->

Untuk mengantisipasi masalah seperti ini, kita perlu memindahkan secara berkala/membuat ulang *titik reset* setiap kali melakukan *upgrade*. Sehingga ketika kita melakukan *factory reset* akan tetap berada di versi yang sedang berjalan, tidak turun/mundur terlalu jauh ke belakang.

## Implementasi di Tumbleweed

Karena saya menggunakan openSUSE Tumbleweed, ini yang biasa saya lakukan untuk memindahkan *titik reset* secara berkala. Ini juga bisa diimplementasikan di openSUSE Leap.

Saya membuat ulang *titik reset* setiap 4 bulan atau 2 bulan sekali. Jika 4 bulan sekali, yaitu setiap rilis **KDE Plasma** baru (5.18.0, 5.19.0, 5.20.0, dan seterusnya). Jika 2 bulan sekali, yaitu setiap rilis **KDE Plasma** baru dan **KDE Applications** baru (20.04.0, 20.08.0, 20.12.0, dan seterusnya). **KDE Plasma** rilis setiap bulan Februari, Juni dan Oktober. Sedangkan **KDE Applications** rilis setiap bulan April, Agustus dan Desember. Untuk pengguna openSUSE Leap bisa melakukannya setahun sekali, setiap rilis openSUSE Leap versi baru (15.0, 15.1, 15.2, 15.3, dan seterusnya).

## Persiapan

### Pindahkan cache zypp

Saya biasanya memindahkan direktori cache zypp dari /var/cache/zypp ke partisi lain di luar sistem. Jika Anda membaca tulisan [minimal/*custom* install openSUSE]({{site.baseurl}}/2020/08/23/minimal-custom-install-opensuse.html) di bagian [expert partitioner]({{site.baseurl}}/2020/08/23/minimal-custom-install-opensuse.html#expert-partitioner), saya punya sebuah HDD (/dev/sdb dengan partisi /dev/sdb1) untuk menyimpan data, di sanalah saya menyimpan semua cache zypp. Untuk memindahkan cache zypp ini kita bisa mengaturnya di /etc/zypp/zypp.conf pada konfigurasi `Path where the cache are kept.` Nilai *default* di sana adalah `/var/cache/zypp`. Saya mengubahnya menjadi `/home/data/cache/zypp` dengan perintah:

`su -c "sed -i 's/# cachedir = \/var/cachedir = \/home\/data' /etc/zypp/zypp.conf"`

### *Backup* konfigurasi dan data penting

Setiap mengubah konfigurasi di /etc, saya biasanya menyalin perubahan tersebut ke partisi data. Dan ketika melakukan *factory reset*, saya menyalin konfigurasi tersebut kembali ke /etc setelah melakukan *factory reset* dan sebelum membuat *titik reset* baru, supaya perubahan ini tidak hilang lagi ketika melakukan *factory reset* berikutnya. Untuk data, saya memang tidak pernah menyimpan data di direktori $HOME. Dan sebelum melakukan *factory reset* saya juga menyalin semua konfigurasi di direktori $HOME ke partisi data:

`rsync -vaHAX --delete $HOME/ /home/data/home-backup/`

Beberapa konfigurasi tersebut akan saya kembalikan ke direktori $HOME setelah membuat *titik reset* baru dan memasang kembali aplikasi pemilik konfigurasi tersebut (seperti Web Browser, Telegram, dan sebagainya). Untuk konfigurasi dari aplikasi yang tidak terlalu ribet, saya memilih mengkonfigurasi ulang (seperti Dolphin, Gwenview, Okular, dan sebagainya).

### Membuat skrip instalasi paket

Untuk memudahkan instalasi semua paket yang saya gunakan setelah membuat *titik reset* baru, saya membuat sebuah skrip `instalasi-paket` yang dibuat *executable* dengan isi:

```
#!/bin/bash

zypper install plasma5-session-wayland sddm-branding-upstream <nama-paket-3> <nama-paket-4> <nama-paket-sdb>
```

Setelah membuat *titik reset* baru, saya tinggal menjalankan skrip tersebut dengan:

`su -c "./instalasi-paket"`

## Proses *factory reset*

### Unduh semua paket *update*/*upgrade*

Karena saya mematikan *autorefresh* repositori, sebelum melakukan *update* saya harus *refresh* manual semua repositori:

`su -c "zypper refresh"`

Setelah semua repositori berhasil diperbarui, lanjutkan dengan mengunduh semua paket menggunakan `zypper dup` dengan tambahan opsi `--download-only`:

`su -c "zypper dup --download-only"`

Dengan perintah tersebut, semua paket yang akan diperbarui/*update* hanya akan diunduh dan tidak dipasang. Semua paket tersebut akan masuk ke direktori cache zypp yang lokasinya sudah diubah, yaitu /home/data/cache/zypp, dan direktori ini tidak akan ikut direset ketika kita melakukan *factory reset*.

Untuk pengguna openSUSE Leap ketika akan melakukan upgrade, sebelum menjalankan `zypper refresh` dan `zypper dup --download-only`, ubah terlebih dahulu repositori ke versi openSUSE Leap tujuan *upgrade* dengan mengubah angkanya (misalnya dari 15.2 ke 15.3):

`su -c "sed -i 's/15.2/15.3/g' /etc/zypp/repos.d/*"`

Jika repositori Anda menggunakan variabel `$releasever`, ubah menjadi angka:

`su -c "sed -i 's/\$releasever/15.3/g' /etc/zypp/repos.d/*"`

### Lakukan *factory reset*

Setelah semua paket *update* berhasil diunduh, jalankan ulang/*reboot* komputer dan masuk ke Kernel terlama dengan parameter kernel tambahan untuk masuk ke CLI:

1. Restart/reboot komputer
2. Di layar Grub2 untuk memilih sistem operasi yang akan dijalankan, pilih **Advanced options for openSUSE**
3. Arahkan kernel terlama/terbawah (tanpa teks *recovery mode*)
4. Tekan tombol **e** pada keyboard untuk mengubah parameter kernel
5. Arahkan ke baris dengan awal teks **linuxefi** atau **linux**
6. Tekan tombol **End** pada keyboard untuk membawa kursor ke akhir teks
7. Tambahkan spasi dan angka **3**
8. Tekan tombol **F10** untuk *booting*

Proses tersebut akan membawa kita ke mode CLI, dari sini kita lakukan *factory reset*. Login, lalu cari tahu *titik reset* sebelumnya.

``su -c 'for config in `. /etc/sysconfig/snapper; echo $SNAPPER_CONFIGS`; do snapper -c $config list; done' | grep 'reset=yes'``

Lihat nomor Snapshot dari *titik reset* terakhir (paling bawah). Jika kita belum pernah melakukan *factory reset* sebelumnya, maka *titik reset* hanya satu, yaitu angka 1.

``su -c 'for config in `. /etc/sysconfig/snapper; echo $SNAPPER_CONFIGS`; do snapper -c $config undochange 1..0'``

Ubah angka 1 dengan angka Snapshot dari *titik reset* terakhir jika Anda pernah mengubah *titik reset* sebelumnya. Setelah selesai, jalankan ulang/*reboot* komputer.

### Lakukan *update*/*upgrade*

Periksa jika opsi `Path where the caches are kept` kembali ke *default* (/var/cache/zypp). Jika kembali, ubah lagi dengan perintah seperti [di atas](#pindahkan-cache-zypp). Jika Anda menggunakan openSUSE Leap, [ubah kembali repositori ke versi tujuan *upgrade*](#unduh-semua-paket-update-upgrade). Karena setelah proses *factory reset* tadi, repositori akan berubah ke asal. Setelah selesai, jalankan proses *update*/*upgrade* tanpa opsi `--download-only`:

`su -c "zypper dup"`

Proses ini tidak akan mengunduh paket, karena semua paket sudah diunduh sebelumnya. Dan juga tidak perlu didahului oleh `zypper refresh`, karena repositori sudah terbaru dan kita tidak terhubung ke internet.

Setelah selesai, jalankan ulang/*reboot* komputer.

### Bersihkan kernel nama dan paket *sampah*

Setelah komputer dijalankan ulang, kita akan kembali ke mode CLI. Lihat daftar kernel yang terpasang:

`zypper search -si kernel-default`

Sekarang kernel yang sedang digunakan adalah menjadi kernel terlama. Maka hapus semua kernel yang lebih lama:

`su -c "zypper remove kernel-default-<versi-kernel>"`

Ganti `<versi-kernel>` dengan angka yang tampil pada kolom `Version` lengkap dengan tanda titik dan tanda garis.

Setelah menghapus kernel lama, hapus juga paket-paket yang sudah tidak dibutuhkan. Cari tahu dengan:

`zypper packages --unneeded --orphaned`

Jika ada, hapus dengan:

`su -c "zypper remove <nama-paket>"`

Setelah selesai, jalankan ulang/*reboot* komputer.

### Kembalikan konfigurasi

Jika Anda pernah mengubah konfigurasi di /etc dan terhapus kembali saat melakukan *factory reset*, [kembalikan konfigurasi tersebut ke /etc](#backup-konfigurasi-dan-data-penting) sebelum membuat *titik reset* baru jika tidak ingin kembali hilang saat melakukan *factory reset* berikutnya.

### Buat titik reset baru

Setelah komputer dijalankan ulang dan login, lihat nomor Snapshot yang baru dibuat saat *booting*:

``su -c 'for config in `. /etc/sysconfig/snapper; echo $SNAPPER_CONFIGS`; do snapper -c $config list; done``

Lihat nomor Snapshot terakhir, lalu buat Snapshot tersebut sebagai *titik reset* baru:

``su -c 'for config in `. /etc/sysconfig/snapper; echo $SNAPPER_CONFIGS`; do snapper -c $config modify -c "" -d "factory reset" -u "reset=yes" <nomor-snapshot>; done'``

Ubah `<nomor-snapshot>` dengan Snapshot terakhir yang diketahui dari perintah sebelumnya.

Lalu hapus *titik reset* lama:

``su -c 'for config in `. /etc/sysconfig/snapper; echo $SNAPPER_CONFIGS`; do snapper -c $config modify -c timeline 1; done'``

Ganti nomor `1` dengan nomor *titik reset* yang lain jika Anda pernah melakukan *factory reset* dan membuat *titik reset* baru sebelumnya.

### Pasang kembali software yang dibutuhkan

Setelah membuat *titik reset* baru, kita tinggal memasang kembali paket-paket yang kita gunakan sehari-hari dengan [menjalankan skrip yang dibuat sebelumnya](#membuat-skrip-instalasi-paket).

Pindah ke direktori di mana skrip berada:

`cd /home/data`

Jika skrip tersebut berada di /home/data.

Jalankan:

`su -c "./instalasi-paket"`

Atau jika tanpa pindah direktori terlebih dahulu:

`su -c "/home/data/instalasi-paket"`

### Kembalikan konfigurasi aplikasi

Kembalikan konfigurasi di direktori $HOME yang sebelumnya di-*backup*. Anda bisa hanya mengembalikan konfigurasi yang cukup merepotkan untuk dikonfigurasi ulang (seperti Web Browser atau Telegram), atau bisa juga mengembalikan semua konfigurasi dengan perintah yang sama ketika melakukan *backup* dengan membalikkan sumber dan tujuannya:

`rsync -vaHAX --delete /home/data/home-backup/ $HOME/`

Jika terjadi konflik antara konfigurasi lama dengan software versi terbaru, kembalikan *subvolume* /home ke *factory reset* baru, lalu buat konfigurasi baru:

`su -c "snapper -c home undochange <nomor-snapshot>..0"`

## Perhatian!

Pada perintah-perintah di atas, saat menjalankan perintah dengan awalan `su -c` ada yang menggunakan tanda kutip ganda dan ada yang menggunakan tanda kutip tunggal. Perintah dengan tanda kutip ganda jika diganti dengan tanda kutip tunggal akan bekerja dengan normal. Tapi jika perintah dengan tanda kutip tunggal diganti dengan tanda kutip ganda, tidak semua bisa bekerja seperti seharusnya. Silakan dicoba.

