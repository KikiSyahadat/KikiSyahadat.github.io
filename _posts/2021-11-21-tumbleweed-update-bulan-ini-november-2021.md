---
title:  Tumbleweed update bulan ini, November 2021
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 24 Oktober 2021, 4 minggu yang lalu, di *Snapshot* **20211021**. Dan di *update* kali ini saya mendapatkan *Snapshot* **20211118**. Total paket yang diperbarui adalah 406 paket di-*upgrade*, 14 paket baru dan 4 paket dihapus dengan total ukuran *download* sebesar **508,5 MiB**.

<!--more-->

Di antara *update* sebelumnya ke *update* kali ini saya memasang paket `phonon4qt5-backend-vlc` supaya bisa memainkan video di **Gwenview** dan panel informasi **Dolphin**. Juga karena *update* sebelumnya saya melakukan *factory reset*, saya juga menghapus paket-paket yang sudah tidak diperlukan lagi oleh sistem.

Untuk melihat paket apa saja yang sudah tidak diperlukan oleh sistem dan/atau sudah tidak ada lagi di repositori, kita bisa menjalankan perintah `zypper packages --unneeded --orphaned`. Lalu menghapus paket-paket tersebut dengan perintah `su -c "zypper remove nama-paket`.

Dan berikut adalah rincian dari *update* kali ini:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 406 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 aaa_base accountsservice ark attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bind-utils bluedevil5 bluez bluez-qt-imports bluez-qt-udev boost-license1_77_0 breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules busybox busybox-psmisc coreutils cpio cpp11 dhcp dhcp-client dolphin dolphin-part drkonqi5 ebtables elfutils ffmpegthumbs file file-magic findutils fprintd fprintd-pam frameworkintegration-plugin gawk gdk-pixbuf-loader-rsvg gdk-pixbuf-query-loaders gio-branding-openSUSE girepository-1_0 git-core glib2-tools gmenudbusmenuproxy grub2 grub2-i386-pc gtk3-data gtk3-metatheme-breeze gtk3-schema gtk3-tools gwenview5 iproute2 iptables kactivities5-imports kactivitymanagerd kate kate-plugins kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kexec-tools kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 kmod knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kquickcharts kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kwalletd5 kwayland kwin5 layer-shell-qt5 libAppStreamQt2 libIex-3_1-30 libIlmThread-3_1-30 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kipi32_0_0 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKScreenLocker5 libKSysGuardSystemStats1 libKWaylandServer5 libLLVM13 libOpenEXR-3_1-30 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Network5 libQt5PrintSupport5 libQt5QuickControls2-5 libQt5QuickTemplates2-5 libQt5Sql5 libQt5Sql5-sqlite libQt5Svg5 libQt5Test5 libQt5TextToSpeech5 libQt5VirtualKeyboard5 libQt5WaylandClient5 libQt5Widgets5 libQt5Xml5 libQtQuick5 libSDL2-2_0-0 libapparmor1 libappstream4 libarchive13 libasm1 libatk-1_0-0 libaudit1 libaugeas0 libavahi-client3 libavahi-common3 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libblkid1 libbluetooth3 libboost_thread1_77_0 libbreezecommon5-5 libbtrfs0 libcairo-gobject2 libcairo2 libdcerpc-binding0 libdcerpc0 libdolphinvcs5 libdw1 libebtc0 libeconf0 libeditorconfig0 libelf1 libell0 libexiv2-27 libfdisk1 libfdk-aac2 libfido2-1 libfreebl3 libfribidi0 libgbm1 libgcc_s1 libgdk_pixbuf-2_0-0 libgio-2_0-0 libgirepository-1_0-1 libglib-2_0-0 libglvnd libgmodule-2_0-0 libgnutls30 libgobject-2_0-0 libgomp1 libgpg-error0 libgstphotography-1_0-0 libgtk-3-0 libinput10 libip4tc2 libip6tc2 libjpeg8 libjson-glib-1_0-0 libkaccounts2 libkdecorations2-5 libkdecorations2private9 libkerfuffle21 libkioarchive5 libkipi-data libkmod2 libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 libldb2 libmagic1 libmount1 libmpg123-0 libncurses6 libndr-krb5pac0 libndr-nbt0 libndr-standard0 libndr2 libnetapi0 libopenmpt0 libopenssl1_1 libpcre2-16-0 libpcre2-8-0 libpipewire-0_3-0 libplist-2_0-3 libpostproc55_9 libpython3_8-1_0 libqca-qt5-2 libqt5-qtquickcontrols2 libqt5-qtvirtualkeyboard libqt5-qtwebengine librav1e0 libre2-9 librsvg-2-2 librtmp1 libsamba-credentials1 libsamba-errors0 libsamba-hostconfig0 libsamba-passdb0 libsamba-util0 libsamdb0 libseccomp2 libselinux1 libsemanage-conf libsemanage2 libsepol2 libshaderc_shared1 libsmartcols1 libsmbclient0 libsmbconf0 libsmbldap2 libsnappy1 libsoftokn3 libspeex1 libssh-config libssh4 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtasn1-6 libteamdctl0 libtevent-util0 libubsan1 libudev1 libusb-1_0-0 libuuid1 libvlc5 libvlccore9 libvo-amrwbenc0 libwacom-data libwacom2 libwbclient0 libx264-161 libx265-199 libxml2-2 libxslt1 libxtables12 libxvidcore4 libzypp logrotate metatheme-breeze-common milou5 mobipocket mozilla-nss mozilla-nss-certs ncurses-utils obs-studio okular openSUSE-release openSUSE-release-appliance-custom otpclient pam pam_unix-nis plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit polkit-kde-agent-5 powerdevil5 prison-qt5-imports python3-bind python38 python38-base qca-qt5 qtdeclarative-imports-provides-qt5 rpm rpm-config-SUSE samba-libs sg3_utils solid-imports sonnet spectacle suse-module-tools syntax-highlighting sysconfig sysconfig-netconfig systemd systemd-rpm-macros systemd-sysvinit systemsettings5 sysvinit-tools terminfo-base timezone udev util-linux util-linux-systemd vlc vlc-noX vlc-qt wicked wicked-service xdg-desktop-portal-kde xembedsniproxy xen-libs xf86-input-libinput xorg-x11-server xorg-x11-server-Xvfb xtables-plugins

The following product is going to be upgraded:
openSUSE Tumbleweed
  20211021-0 -> 20211118-0

The following 14 NEW packages are going to be installed:
  alts iso-codes kernel-default-5.15.2-1.1 libSPIRV-Tools-suse23 libZXing1 libalternatives1 libexslt0 libgit2-1_3 libmaxminddb0 libpolkit-agent-1-0 libpolkit-gobject-1-0 libsgutils2-1_47-2 libxcvt0 v4l2loopback-kmp-default-0.12.5_k5.15.2_1-5.51

The following 4 packages are going to be REMOVED:
  libSPIRV-Tools-suse22 libgit2-1_2 libpolkit0 libsgutils2-1_46-2

The following package requires a system reboot:
  kernel-default-5.15.2-1.1

406 packages to upgrade, 14 new, 4 to remove.
Overall download size: 508.5 MiB. Already cached: 0 B. After the operation, additional 201.5 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* selanjutnya adalah sekitar tanggal 19 Desember 2021, 4 minggu dari sekarang.

