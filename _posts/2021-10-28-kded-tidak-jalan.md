---
title:  KDED tidak jalan
tags:
  - KDE
  - openSUSE
  - Troubleshooting
  - Tumbleweed
---

Saya biasanya melakukan [factory reset]({{site.baseurl}}/2020/09/03/membuat-fitur-factory-reset.html) setiap empat bulan sekali. Atau lebih tepatnya setiap rilis Plasma terbaru. Dan di update bulan ini, Plasma 5.23 rilis, yang artinya saatnya saya melakukan *factory reset*. Namun masalah terjadi.

<!--more-->

Ketika selesai melakukan *update*, lalu saya *install* semua paket/*software*/aplikasi yang saya butuhkan, lalu *reboot*, ada beberapa fitur yang tidak jalan. Di antaranya, di pengaturan **System Settings** >> **Appearance** >> **Global Theme** >> **Application Style**, opsi **Configure GNOME/GTK Application Style** tidak muncul.

Lalu di pengaturan **System Settings** >> **Startup and Shutdown** >> **Background Service** muncul peringatan `The background service manager (kded5) is currently not running. Make sure it is installed correctly.` Dan semua **Startup Service** di layar tersebut tidak jalan.

Lalu ketika saya menambahkan *layout* *keyboard* di pengaturan **System Settings** >> **Input Device** >> **Keyboard** >> **Layout** tidak membuat indikator *keyboard* otomatis muncul di **System Tray**. Bahkan ketika saya mencoba mengubah *layout* dengan *shortcut* pun tidak membuat *layout* berubah.

Dan yang lebih penting adalah ketika saya mencoba menghubungkan laptop dengan monitor eksternal, saya tidak bisa mengaktifkannya. Padahal di hari Senin malam (malam Selasa) saya diminta oleh kakak saya untuk melakukan [*live streaming* haul pertama anaknya (keponakan saya)](https://www.youtube.com/watch?v=WhtnWcEUg5Q){:target="_blank"}. Dan fitur ini akan sangat dibutuhkan saat itu.

Dan yang terakhir adalah **Global Menu** juga tidak bisa diaktifkan.

Akhirnya saya membatalkan *factory reset* saat itu untuk kemudian dicari akar masalahnya setelah urusan saya selesai.

Setelah saya cari tahu, ternyata masalahnya adalah paket `gsettings-desktop-schemas` yang hilang. Setelah paket tersebut dipasang, semua kembali normal. Dan saya bisa melakukan *factory reset* di bulan ini.

