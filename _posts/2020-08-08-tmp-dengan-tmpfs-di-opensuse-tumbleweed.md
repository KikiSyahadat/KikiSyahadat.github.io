---
title:  /tmp dengan tmpfs di openSUSE Tumbleweed
tags:
  - Informasi
  - openSUSE
  - Panduan
  - tmpfs
  - Tumbleweed
---

Jika Anda memasang openSUSE Tumbleweed dengan versi ISO Snapshot 20200806 secara baku instalasi Anda akan membuat direktori */tmp* dengan *tmpfs*, sedangkan pada versi sebelum Snapshot tersebut */tmp* akan berada pada sebuah *subvolume* Btrfs.

<!--more-->

## Membuat */tmp* dengan *tmpfs* pada instalasi sebelum 20200806

Jika Anda sudah lama menggunakan openSUSE Tumbleweed (instalasi dilakukan sebelum ISO Snapshot 20200806) dan ingin membuat */tmp* berada pada *tmpfs* seperti pada instalasi baru, Anda tinggal menghapus baris mounting */tmp* di */etc/fstab* dengan perintah `su -c "sed -i '/tmp/d' /etc/fstab"`, lalu hapus semua file dan folder yang berada di direktori */tmp* dengan perintah `su -c "rm -rv /tmp/* /tmp/.*"`, setelah itu jalankan ulang komputer.

## Instalasi lama yang sudah menggunakan *tmpfs* untuk */tmp*

Sebelumnya saya pernah membuat tulisan tentang [Memindahkan /tmp ke tmpfs](https://opensuse.id/2019/09/08/memindahkan-tmp-ke-tmpfs/){:target="_blank"}. Jika Anda mengikuti tulisan tersebut, segera hapus link */etc/systemd/system/tmp.mount* dengan `su -c "rm -v /etc/systemd/system/tmp.mount"` setelah Anda melakukan update Tumbleweed ke versi 20200806, karena di versi tersebut file */usr/share/systemd/tmp.mount* sudah tidak ada. Jadi bisa dipastikan link tersebut akan terputus.

Jangan lupa juga untuk memastikan bahwa di */etc/fstab* sudah tidak ada baris mounting */tmp*.

