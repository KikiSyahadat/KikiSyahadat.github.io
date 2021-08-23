---
title:  Tumbleweed update bulan ini, Agustus 2021
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan di tanggal 18 Juli 2021, 5 minggu yang lalu, di *Snapshot* **20210715**. Rencananya saya akan melakukan *update* di hari Minggu, 22 Agustus 2021 di *Snapshot* **20210817**. Tapi ketika akan dilakukan *update*, saya lihat banyak sekali paket baru yang harus ikut dipasang. Akhirnya saya urungkan dan memutuskan untuk menunggu *Snapshot* berikutnya.

<!--more-->

Tapi ketika hari ini saya coba *update* lagi ke *Snapshot* **20210820** yang baru rilis tadi malam, hasilnya sama saja, banyak paket baru yang ikut dipasang. Akhirnya saya putuskan untuk melakukan *update* ke *Snapshot* **20210817** kemarin dengan terlebih dahulu melakukan `zypper addlock patterns-microos-desktop-common`, karena inilah penyebab banyaknya paket baru yang mesti ikut dipasang.

Dan di *Snapshot* **20210817** ini, total paket yang diperbarui adalah 404 paket di-*upgrade*, 1 paket di-*downgrade*, 6 paket baru dan 4 paket dihapus, dengan total ukuran *download* sebesar **446,8 MiB**.

Seandainya saya tidak melakukan `addlock`, total paket yang diperbarui akan jadi sebanyak 401 paket di-*upgrade*, 1 paket di-*downgrade*, 154 paket baru dan 8 paket dihapus, dengan total ukuran *download* sebesar **523,9 MiB**.

Dan detailnya seperti berikut:

```
user@opensuse:~> su -c "zypper dup"
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following item is locked and will not be changed by any action:
 Available:
  patterns-microos-desktop-common

The following 6 NEW packages are going to be installed:
  kernel-default-5.13.8-1.1 libgps29 libliveMedia97 libmbedcrypto7 libqalculate22 v4l2loopback-kmp-default-0.12.5_k5.13.8_1-5.29

The following 4 packages are going to be REMOVED:
  libgps28 libliveMedia94 libmbedcrypto6 libqalculate21

The following 404 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 NetworkManager NetworkManager-branding-openSUSE NetworkManager-openvpn aaa_base ark at-spi2-core attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bash bind-utils bluedevil5 bluez bluez-qt-imports bluez-qt-udev breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules busybox-psmisc ca-certificates cpp cpp11 dhcp dhcp-client diffutils dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 e2fsprogs ffmpegthumbs filesystem firewalld frameworkintegration-plugin gdk-pixbuf-loader-rsvg gdk-pixbuf-query-loaders girepository-1_0 glib2-tools gmenudbusmenuproxy grep grub2 grub2-i386-pc gstreamer-plugins-base gtk3-data gtk3-metatheme-breeze gtk3-schema gtk3-tools gwenview5 hwdata iproute2 ipset iputils irqbalance kactivities5-imports kactivitymanagerd kate kate-plugins kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kquickcharts kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kwalletd5 kwayland kwin5 layer-shell-qt5 less libAppStreamQt2 libBasicUsageEnvironment1 libHalf-2_5-25 libIex-2_5-25 libIlmImf-2_5-25 libIlmThread-2_5-25 libImath-2_5-25 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kipi32_0_0 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKScreenLocker5 libKSysGuardSystemStats1 libKWaylandServer5 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Network5 libQt5PrintSupport5 libQt5Sql5 libQt5Sql5-sqlite libQt5Test5 libQt5Widgets5 libQt5Xml5 libSDL2-2_0-0 libUsageEnvironment3 libXfont2-2 libXft2 libaom3 libapparmor1 libappstream4 libatspi0 libaudit1 libavahi-client3 libavahi-common3 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libbluetooth3 libbreezecommon5-5 libbtrfs0 libcap2 libcfitsio9 libcom_err2 libcrypt1 libcurl4 libdav1d5 libdcerpc-binding0 libdcerpc0 libdevmapper1_03 libdolphinvcs5 libext2fs2 libfdk-aac2 libfreebl3 libfreetype6 libgbm1 libgcc_s1 libgdk_pixbuf-2_0-0 libgio-2_0-0 libgirepository-1_0-1 libgit2-1_1 libglib-2_0-0 libglvnd libgmodule-2_0-0 libgobject-2_0-0 libgomp1 libgpgme11 libgpgmepp6 libgroupsock30 libgstallocators-1_0-0 libgstapp-1_0-0 libgstaudio-1_0-0 libgstgl-1_0-0 libgstpbutils-1_0-0 libgstphotography-1_0-0 libgstriff-1_0-0 libgsttag-1_0-0 libgstvideo-1_0-0 libgtk-3-0 libharfbuzz-subset0 libharfbuzz0 libibus-1_0-5 libidn12 libidn2-0 libinput10 libipset13 libixml11 libkaccounts2 libkdecorations2-5 libkdecorations2private8 libkerfuffle21 libkeyutils1 libkioarchive5 libkipi-data libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 liblua5_4-5 libmbedtls13 libmbedx509-1 libmozjs-78-0 libncurses6 libndr-krb5pac0 libndr-nbt0 libndr-standard0 libndr1 libnetapi0 libnm0 libnuma1 libogg0 libopenssl1_1 libpackagekitqt5-1 libpango-1_0-0 libpcre1 libpipewire-0_3-0 libpolkit-qt5-1-1 libpolkit0 libpoppler-qt5-1 libpoppler111 libpostproc55_9 libprotobuf-lite28 libproxy1 libpulse-mainloop-glib0 libpulse0 libpython3_8-1_0 libqt5-qtwebengine librav1e0 libre2-9 librsvg-2-2 libsamba-credentials1 libsamba-errors0 libsamba-hostconfig0 libsamba-passdb0 libsamba-util0 libsamdb0 libselinux1 libsepol2 libsmbclient0 libsmbconf0 libsmbldap2 libsnappy1 libsndfile1 libsoftokn3 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtevent-util0 libubsan1 libudev1 libupnp17 libvlc5 libvlccore9 libwbclient0 libzypp metatheme-breeze-common milou5 mobipocket mozilla-nspr mozilla-nss mozilla-nss-certs ncurses-utils netcfg numactl obs-studio okular openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common openvpn pam pam_unix-nis perl-Bootloader plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit polkit-kde-agent-5 powerdevil5 prison-qt5-imports pulseaudio pulseaudio-module-bluetooth pulseaudio-module-x11 pulseaudio-utils python3-bind python3-firewall python38 python38-base python38-dbus-python python38-decorator python38-gobject samba-libs samba-libs-python3 sddm sddm-branding-upstream solid-imports sonnet spectacle syntax-highlighting systemd systemd-sysvinit systemsettings5 sysuser-shadow terminfo-base timezone typelib-1_0-NM-1_0 udev vlc vlc-noX vlc-qt whois xdg-desktop-portal-kde xembedsniproxy xen-libs xkeyboard-config xorg-x11-server xorg-x11-server-Xvfb zypper

The following product is going to be upgraded:
openSUSE Tumbleweed
  20210715-0 -> 20210817-0

The following package is going to be downgraded:
  libluajit-5_1-2

The following package requires a system reboot:
  kernel-default-5.13.8-1.1

404 packages to upgrade, 1 to downgrade, 6 new, 4 to remove.
Overall download size: 446.8 MiB. Already cached: 0 B. After the operation, additional 193.8 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y):
```

Di antara *update* sebelumnya dengan *update* kali ini saya melakukan beberapa perubahan, di antaranya memasang paket `v4l2loopback-kmp-default` untuk fitur **Virtual Camera** di **OBS Studio** dan menghapus paket `tlp`, `smartmontools`, `ethtool`, `acpi_call` dan `acpi_call-kmp-default`.

Jadwal *update* berikutnya adalah sekitar tanggal 19 September 2021, 4 minggu dari sekarang.

