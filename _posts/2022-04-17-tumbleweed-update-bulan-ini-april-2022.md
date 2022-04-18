---
title:  Tumbleweed update bulan ini, April 2022
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 20 Maret 2022, 4 pekan yang lalu di *Snapshot* **20220318**. Dan di *update* kali ini saya mendapatkan *Snapshot* **20220414**. Total paket yang diperbarui adalah: 383 paket di-*upgrade*, 3 paket baru dan 1 paket dihapus dengan total ukuran *download* sebesar **545,6 MiB**.

<!--more-->

Berikut adalah rincian *update* kali ini:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 383 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 NetworkManager NetworkManager-branding-openSUSE aaa_base accountsservice at-spi2-core attica-qt5 baloo5-imports baloo5-kioslaves bash bash-sh bind-utils bluedevil5 bluez bluez-qt-imports bluez-qt-udev breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style busybox busybox-psmisc cpp cpp11 cups-config dbus-1 dhcp dhcp-client dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 file file-magic firewalld frameworkintegration-plugin gawk gdk-pixbuf-loader-rsvg gdk-pixbuf-query-loaders gio-branding-openSUSE girepository-1_0 glib2-tools gmenudbusmenuproxy gpg2 grub2 grub2-i386-pc gsettings-desktop-schemas gstreamer gstreamer-plugins-base gtk3-data gtk3-metatheme-breeze gtk3-schema gtk3-tools gwenview5 gzip iproute2 kactivities5-imports kactivitymanagerd kate kate-plugins kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 kmod knewstuff knewstuff-imports kpackage kpeople5 kquickcharts krb5 kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kuserfeedback-imports kwalletd5 kwayland kwin5 layer-shell-qt5 libAppStreamQt2 libIex-3_1-30 libIlmThread-3_1-30 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KDELibs4Support5 libKF5KHtml5 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5Syndication5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5UnitConversion5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKScreenLocker5 libKSysGuardSystemStats1 libKUserFeedbackCore1 libKUserFeedbackWidgets1 libKWaylandServer5 libLLVM13 libOpenEXR-3_1-30 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Network5 libQt5PrintSupport5 libQt5Sql5 libQt5Sql5-sqlite libQt5Test5 libQt5Widgets5 libQt5Xml5 libQtQuick5 libX11-6 libX11-data libX11-xcb1 libXcursor1 libapparmor1 libappstream4 libarchive13 libatk-1_0-0 libatspi0 libaudit1 libaugeas0 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libbluetooth3 libbluray2 libbreezecommon5-5 libcfitsio9 libcolord2 libcups2 libcurl4 libdbus-1-3 libdevmapper1_03 libdolphinvcs5 libdouble-conversion3 libeconf0 libepoxy0 libevdev2 libexpat1 libfdk-aac2 libfido2-1 libfreebl3 libfreetype6 libgbm1 libgcc_s1 libgdk_pixbuf-2_0-0 libgio-2_0-0 libgirepository-1_0-1 libglib-2_0-0 libglslang11 libgmodule-2_0-0 libgnutls30 libgobject-2_0-0 libgomp1 libgraphene-1_0-0 libgstallocators-1_0-0 libgstapp-1_0-0 libgstaudio-1_0-0 libgstgl-1_0-0 libgstpbutils-1_0-0 libgstphotography-1_0-0 libgstreamer-1_0-0 libgstriff-1_0-0 libgsttag-1_0-0 libgstvideo-1_0-0 libgtk-3-0 libharfbuzz-subset0 libharfbuzz0 libibus-1_0-5 libjpeg8 libkdecorations2-5 libkdecorations2private9 libkioarchive5 libkmod2 libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 libldb2 liblirc_client0 libltdl7 libmagic1 libminizip1 libmnl0 libncurses6 libnfnetlink0 libnghttp2-14 libnm0 libopenmpt0 libphonon4qt5 libpipewire-0_3-0 libpoppler119 libpostproc55_9 libprocps8 libprotobuf-lite30 libpython3_8-1_0 libqt5-qtwebengine libre2-9 librsvg-2-2 librtmp1 libsasl2-3 libshaderc_shared1 libsigc-2_0-0 libslp1 libsnapper5 libsndfile1 libsoftokn3 libsolv-tools libsqlite3-0 libsratom-0-0 libsrt1_4 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtdb1 libubsan1 libudev1 libunistring2 libupower-glib3 libvlc5 libvlccore9 libvmaf1 libvo-amrwbenc0 libx264-161 libx265-199 libxml2-2 libxvidcore4 libz1 libzypp metatheme-breeze-common milou5 mozilla-nss mozilla-nss-certs ncurses-utils obs-studio openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common otpclient perl-Bootloader phonon4qt5-backend-vlc pipewire-modules-0_3 pipewire-spa-plugins-0_2 plasma-framework plasma-framework-components plasma-nm5 plasma5-addons plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit-kde-agent-5 powerdevil5 prison-qt5-imports procps purpose python3-bind python3-firewall python38 python38-base rpm-config-SUSE samba-client-libs setxkbmap shared-mime-info snapper solid-imports sonnet syntax-highlighting system-user-srvGeoClue systemd systemd-sysvcompat systemsettings5 terminfo-base timezone typelib-1_0-NM-1_0 udev upower vlc vlc-noX vlc-qt whois xdg-desktop-portal xdg-desktop-portal-kde xdm xdpyinfo xembedsniproxy xen-libs xorg-x11-server xorg-x11-server-Xvfb xterm-bin xterm-resize

The following product is going to be upgraded:
openSUSE Tumbleweed
  20220318-0 -> 20220414-0

The following 3 NEW packages are going to be installed:
  kernel-default-5.17.2-1.1 libldap2 v4l2loopback-kmp-default-0.12.5_k5.17.2_1-6.5

The following package is going to be REMOVED:
  libldap-2_4-2

The following package requires a system reboot:
  kernel-default-5.17.2-1.1

383 packages to upgrade, 3 new, 1 to remove.
Overall download size: 545.6 MiB. Already cached: 0 B. After the operation, additional 266.3 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* berikutnya adalah sekitar tanggal 22 Mei 2022, 5 pekan dari sekarang.

