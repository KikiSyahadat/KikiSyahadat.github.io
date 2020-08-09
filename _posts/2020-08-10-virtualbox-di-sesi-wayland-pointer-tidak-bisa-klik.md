---
title:  VirtualBox di sesi Wayland, pointer tidak bisa klik
tags:
  - Linux
  - Troubleshooting
  - VirtualBox
  - Wayland
---

Ini saya alami di Plasma 5 Wayland. Ketika saya menjalankan Guest OS di VirtualBox, pointer (Touchpad/Mouse) hanya berfungsi saat klik pertama, klik selanjutnya tidak berefek sama sekali. Bahkan ketika saya berpindah ke aplikasi lain (dengan Alt + Tab), pointer klik juga menjadi ikut tidak berfungsi. Cara satu-satunya supaya kembali berfungsi adalah dengan *membunuh* Guest OS yang sedang berjalan.

<!--more-->

## Situasi

1. Login ke sesi Wayland.
2. Buka menu utama VirtualBox lewat menu desktop.
3. Jalankan salah satu Guest OS.
4. Klik di manapun di dalam Guest OS (contoh: di menu). Klik pertama biasanya berjalan normal, klik berikutnya tidak akan berfungsi, baik klik kiri atau pun klik kanan.

## Solusi

1. Matikan Guest OS yang sedang berjalan (jika ada) dengan menekan tombol Ctrl + Alt + Esc secara bersamaan. Setelah pointer berubah menjadi gambar tengkorak, klik pada Guest OS.
2. Buka menu utama VirtualBox (jika belum terbuka).
3. Pilih **File** >> **Preferences...**
4. Pilih tab **Input**.
5. Klik **Auto Capture Keyboard** untuk menghilangkan tanda centang (ceklis).
6. Klik **OK**.
7. Coba jalankan salah satu Guest OS.
8. Klik di manapun di dalam Guest OS. Klik pertama dan seterusnya akan berfungsi dengan normal.

