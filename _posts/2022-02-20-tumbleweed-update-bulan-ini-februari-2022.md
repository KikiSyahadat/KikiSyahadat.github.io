---
title:  Tumbleweed update bulan ini, Februari 2022
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 16 Januari 2022, 5 pekan yang lalu di *Snapshot* **20220114**. Dan di *update* kali ini saya mendapatkan *Snapshot* **20220218**. Total paket yang diperbarui adalah: 379 paket di-*upgrade*, 19 paket baru dan 23 paket dihapus dengan total ukuran *download* sebesar **552,1 MiB**.

<!--more-->

Di antara *update* sebelumnya dengan *update* kali ini saya menghapus paket `chromium` dan `virtualbox`.

Juga sebelum melakuan *update* kali ini saya melakukan *factory reset* dan menghapus semua paket *orphaned* dan *unneeded* setelah proses *update* selesai.

Dan berikut adalah rincian *update* kali ini:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 379 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 NetworkManager NetworkManager-branding-openSUSE accountsservice appmenu-gtk-module-common appmenu-gtk3-module ark attica-qt5 baloo5-widgets bash bash-sh bind-utils bluedevil5 bluez breeze breeze5-cursors breeze5-decoration breeze5-style btrfsprogs btrfsprogs-udev-rules busybox-psmisc cpp cpp11 dhcp dhcp-client dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 e2fsprogs ffmpegthumbs findutils firewalld fontconfig gdk-pixbuf-loader-rsvg gio-branding-openSUSE girepository-1_0 git-core glib2-tools glibc glibc-locale-base gmenudbusmenuproxy grep grub2 grub2-i386-pc gstreamer gstreamer-plugins-base gtk3-data gtk3-metatheme-breeze gtk3-schema gtk3-tools gwenview5 gzip iputils iso-codes iso-codes-lang kactivitymanagerd kate kate-plugins kbd kbd-legacy kde-cli-tools5 kde-gtk-config5 kdeclarative-components kdeconnect-kde kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kglobalaccel5 khotkeys5 kinfocenter5 kio kio-core kio-extras5 kmenuedit5 konsole konsole-part krb5 kscreen5 kscreenlocker ksysguardsystemstats-data ksystemstats5 ktexteditor kuserfeedback-imports kwayland kwin5 layer-shell-qt5 libBasicUsageEnvironment1 libIex-3_1-30 libIlmThread-3_1-30 libKF5Attica5 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Completion5 libKF5ConfigWidgets5 libKF5Declarative5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5ItemViews5 libKF5JobWidgets5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kipi32_0_0 libKF5Notifications5 libKF5QuickAddons5 libKF5Screen7 libKF5Solid5 libKF5SyntaxHighlighting5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKScreenLocker5 libKSysGuardSystemStats1 libKUserFeedbackCore1 libKUserFeedbackWidgets1 libKWaylandServer5 libLLVM13 libOpenEXR-3_1-30 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Network5 libQt5PrintSupport5 libQt5QuickControls2-5 libQt5QuickTemplates2-5 libQt5Sql5 libQt5Sql5-sqlite libQt5Svg5 libQt5Test5 libQt5TextToSpeech5 libQt5VirtualKeyboard5 libQt5WaylandClient5 libQt5WebChannel5 libQt5WebChannel5-imports libQt5Widgets5 libQt5X11Extras5 libQt5Xml5 libQtQuick5 libSDL2-2_0-0 libSvtAv1Enc0 libUsageEnvironment3 libapparmor1 libappmenu-gtk3-parser0 libatomic1 libaugeas0 libavahi-client3 libavahi-common3 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libblkid1 libbluetooth3 libbreezecommon5-5 libbtrfs0 libcaca0 libcap2 libcodec2-1_0 libcom_err2 libcryptsetup12 libdevmapper1_03 libdolphinvcs5 libell0 libexpat1 libext2fs2 libfdisk1 libfdk-aac2 libfftw3-3 libfido2-1 libfontconfig1 libfreebl3 libgbm1 libgcc_s1 libgcrypt20 libgdbm6 libgdbm_compat4 libgio-2_0-0 libgirepository-1_0-1 libglib-2_0-0 libglslang11 libglvnd libgmodule-2_0-0 libgnutls30 libgobject-2_0-0 libgomp1 libgpg-error0 libgraphite2-3 libgroupsock30 libgstallocators-1_0-0 libgstapp-1_0-0 libgstaudio-1_0-0 libgstgl-1_0-0 libgstpbutils-1_0-0 libgstphotography-1_0-0 libgstreamer-1_0-0 libgstriff-1_0-0 libgsttag-1_0-0 libgstvideo-1_0-0 libgtk-3-0 libgudev-1_0-0 libharfbuzz-subset0 libharfbuzz0 libhogweed6 libical3 libimobiledevice-1_0-6 libjansson4 libkaccounts2 libkdecorations2-5 libkdecorations2private9 libkerfuffle21 libkioarchive5 libkipi-data libkscreen2-plugin libksysguard5 libksysguard5-imports liblcms2-2 libldb2 liblua5_4-5 libmbedcrypto7 libmbedx509-1 libmount1 libncurses6 libndp0 libnetfilter_conntrack3 libnettle8 libnm0 libopenaptx0 libopenmpt0 libopenssl1_1 libp11-kit0 libpango-1_0-0 libpci3 libpipewire-0_3-0 libplist-2_0-3 libpolkit-agent-1-0 libpolkit-gobject-1-0 libpoppler117 libpostproc55_9 libprocps8 libproxy1 libpulse-mainloop-glib0 libpulse0 libqt5-qdbus libqt5-qtpaths libqt5-qtquickcontrols2 libqt5-qtvirtualkeyboard libqt5-qtwebengine libre2-9 libreadline8 librsvg-2-2 librtmp1 libsasl2-3 libsemanage-conf libsemanage2 libsgutils2-1_47-2 libshaderc_shared1 libsmartcols1 libsnapper5 libsoftokn3 libsolv-tools libsqlite3-0 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtevent0 libubsan1 libudev1 libusb-1_0-0 libuuid1 libuv1 libva-drm2 libva-wayland2 libva-x11-2 libva2 libvlc5 libvlccore9 libvo-amrwbenc0 libwebp7 libwebpdemux2 libwebpmux3 libx264-161 libx265-199 libxkbcommon-x11-0 libxkbcommon0 libxvidcore4 libzstd1 libzypp login_defs metatheme-breeze-common milou5 mobipocket mozilla-nss mozilla-nss-certs ncurses-utils obs-studio okular openSUSE-release openSUSE-release-appliance-custom openvpn otpclient p11-kit p11-kit-tools pam-config perl-Bootloader pipewire-modules-0_3 pipewire-spa-plugins-0_2 plasma-nm5 plasma-nm5-openvpn plasma5-addons plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit polkit-kde-agent-5 powerdevil5 procps pulseaudio pulseaudio-module-bluetooth pulseaudio-module-x11 pulseaudio-setup pulseaudio-utils python3-bind python3-firewall python38-gobject qtdeclarative-imports-provides-qt5 rpm rpm-config-SUSE samba-libs sg3_utils shadow snapper solid-imports spectacle suse-module-tools syntax-highlighting system-user-pulse system-user-root systemd systemd-rpm-macros systemd-sysvinit systemsettings5 sysuser-shadow terminfo-base typelib-1_0-NM-1_0 ucode-intel udev util-linux util-linux-systemd vlc vlc-noX vlc-qt wicked wicked-service wpa_supplicant xdg-desktop-portal xdg-desktop-portal-kde xdm xembedsniproxy xen-libs xf86-input-libinput xorg-x11-server xorg-x11-server-Xvfb zstd zypper

The following product is going to be upgraded:
openSUSE Tumbleweed
  20220114-0 -> 20220218-0

The following 4 packages are going to change vendor:
libgstphotography-1_0-0 
  http://packman.links2linux.de -> openSUSE
libpipewire-0_3-0       
  http://packman.links2linux.de -> openSUSE
pipewire-modules-0_3    
  http://packman.links2linux.de -> openSUSE
pipewire-spa-plugins-0_2
  http://packman.links2linux.de -> openSUSE

The following 19 NEW packages are going to be installed:
  Mesa-demo-x hwdata kernel-default-5.16.8-1.1 libSPIRV-Tools-suse24 libXxf86dga1 libdmx1 libduktape206 libimobiledevice-glue-1_0-0 libliveMedia106 libmbedtls14 libplacebo192 libprotobuf-lite30 libsubid4 pciutils samba-client-libs v4l2loopback-kmp-default-0.12.5_k5.16.8_1-5.64 vulkan-tools wayland-utils xdpyinfo

The following 23 packages are going to be REMOVED:
  libSPIRV-Tools-suse23 libdcerpc-binding0 libdcerpc0 libliveMedia102 libmbedtls13 libndr-krb5pac0 libndr-nbt0 libndr-standard0 libndr2 libnetapi0 libplacebo157 libprotobuf-lite28 libsamba-credentials1 libsamba-errors0 libsamba-hostconfig0 libsamba-passdb0 libsamba-util0 libsamdb0 libsmbclient0 libsmbconf0 libsmbldap2 libtevent-util0 libwbclient0

The following package requires a system reboot:
  kernel-default-5.16.8-1.1

379 packages to upgrade, 19 new, 23 to remove, 4  to change vendor.
Overall download size: 552.1 MiB. Already cached: 0 B. After the operation, additional 283.5 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* selanjutnya adalah sekitar tanggal 20 Maret 2022, 4 pekan dari sekarang.

