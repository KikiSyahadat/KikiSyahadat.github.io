---
title:  Tumbleweed update bulan ini, Juli 2021
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan di tanggal 20 Juni 2021, 4 minggu yang lalu, di *Snapshot* **20210618**. Dan *update* hari ini saya mendapatkan *Snapshot* **20210715**. Total paket yang diperbarui adalah 379 paket di-*upgrade*, 12 paket baru dan 5 paket dihapus, dengan total ukuran *download* sebesar **442,4 MiB**.

Dan detailnya seperti berikut:

<!--more-->

```
user@opensuse:~> su -c "zypper dup"
Swipe your finger across the fingerprint reader
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 12 NEW packages are going to be installed:
  acpi_call-kmp-default-1.1.0_k5.13.1_1-3.368 dracut-mkinitrd-deprecated iio-sensor-proxy kernel-default-5.13.1-1.1 libgroupsock30 libkdsoap2 libliveMedia94 libpoppler111 libprotobuf-lite28 qca-qt5 system-user-srvGeoClue systemd-rpm-macros

The following 5 packages are going to be REMOVED:
  libgroupsock8 libkdsoap1_9_0 libliveMedia81 libpoppler110 libprotobuf-lite26

The following 379 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 NetworkManager NetworkManager-branding-openSUSE aaa_base acpi_call appmenu-gtk-module-common appmenu-gtk3-module ark at-spi2-core attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bind-utils bluedevil5 bluez bluez-qt-imports bluez-qt-udev breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules busybox-psmisc ca-certificates-mozilla compat-usrmerge-tools coreutils cpio cpp11 dolphin dolphin-part dracut drkonqi5 e2fsprogs ffmpegthumbs frameworkintegration-plugin glibc glibc-locale-base gmenudbusmenuproxy grub2 grub2-i386-pc gtk3-metatheme-breeze gwenview5 gzip hwdata irqbalance kactivities5-imports kactivitymanagerd kate kate-plugins kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kquickcharts kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kuserfeedback-imports kwalletd5 kwayland kwin5 layer-shell-qt5 less libAppStreamQt2 libBasicUsageEnvironment1 libGLU1 libHalf-2_5-25 libIex-2_5-25 libIlmImf-2_5-25 libIlmThread-2_5-25 libImath-2_5-25 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kipi32_0_0 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKScreenLocker5 libKSysGuardSystemStats1 libKUserFeedbackCore1 libKUserFeedbackWidgets1 libKWaylandServer5 libLLVM12 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Multimedia5 libQt5Network5 libQt5Positioning5 libQt5PrintSupport5 libQt5QuickControls2-5 libQt5QuickTemplates2-5 libQt5Sensors5 libQt5Sql5 libQt5Sql5-sqlite libQt5Svg5 libQt5Test5 libQt5TextToSpeech5 libQt5VirtualKeyboard5 libQt5WaylandClient5 libQt5WebChannel5 libQt5WebChannel5-imports libQt5Widgets5 libQt5X11Extras5 libQt5Xml5 libQtQuick5 libSDL2-2_0-0 libUsageEnvironment3 libappmenu-gtk3-parser0 libappstream4 libatspi0 libaudit1 libaugeas0 libavahi-client3 libavahi-common3 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libbluetooth3 libbreezecommon5-5 libbtrfs0 libcdio_cdda2 libcdio_paranoia2 libcom_err2 libcryptsetup12 libdevmapper1_03 libdolphinvcs5 libdrm2 libdrm_amdgpu1 libdrm_intel1 libdrm_nouveau2 libdrm_radeon1 libeconf0 libeditorconfig0 libell0 libevdev2 libexiv2-27 libext2fs2 libfdk-aac2 libgbm1 libgcc_s1 libglslang11 libgomp1 libgstphotography-1_0-0 libibus-1_0-5 libkaccounts2 libkdecorations2-5 libkdecorations2private8 libkerfuffle21 libkioarchive5 libkipi-data libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 liblilv-0-0 libluajit-5_1-2 libmozjs-78-0 libmpg123-0 libncurses6 libnm0 libopenmpt0 libpgm-5_2-0 libpipewire-0_3-0 libpkgconf3 libpolkit-qt5-1-1 libpoppler-qt5-1 libpostproc55_9 libprocps8 libprojectM3 libpython3_8-1_0 libqalculate21 libqca-qt5-2 libqt5-qdbus libqt5-qtgraphicaleffects libqt5-qtimageformats libqt5-qtpaths libqt5-qtquickcontrols libqt5-qtquickcontrols2 libqt5-qtvirtualkeyboard libqt5-qtwebengine libsepol2 libserd-0-0 libshaderc_shared1 libsnapper5 libsqlite3-0 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtheora0 libtheoradec1 libtheoraenc1 libubsan1 libudev1 libuv1 libva-drm2 libva-wayland2 libva-x11-2 libva2 libvlc5 libvlccore9 libvmaf1 libvulkan1 libx264-161 libx265-199 libxxhash0 libzck1 libzip5 libzmq5 login_defs metatheme-breeze-common milou5 mobipocket ncurses-utils obs-studio okular openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common pam pam_unix-nis pkgconf pkgconf-m4 pkgconf-pkg-config plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit-kde-agent-5 powerdevil5 prison-qt5-imports procps python3-bind python38 python38-base python38-gobject python38-six qtdeclarative-imports-provides-qt5 rpm-config-SUSE sddm sddm-branding-upstream shadow snapper solid-imports sonnet spectacle suse-module-tools syntax-highlighting sysconfig sysconfig-netconfig system-group-hardware system-group-kvm system-user-lp system-user-nobody systemd systemd-sysvinit systemsettings5 sysuser-shadow terminfo-base typelib-1_0-NM-1_0 udev vlc vlc-noX vlc-qt xdg-desktop-portal-kde xembedsniproxy xf86-input-libinput xorg-x11-server xorg-x11-server-Xvfb xterm-bin

The following product is going to be upgraded:
openSUSE Tumbleweed
  20210618-0 -> 20210715-0

The following package requires a system reboot:
  kernel-default-5.13.1-1.1

379 packages to upgrade, 12 new, 5 to remove.
Overall download size: 442.4 MiB. Already cached: 0 B. After the operation, additional 199.5 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* berikutnya adalah sekitar tanggal 22 Agustus 2021, 5 minggu dari sekarang.

