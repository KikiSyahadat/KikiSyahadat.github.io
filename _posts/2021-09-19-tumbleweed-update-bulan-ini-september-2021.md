---
title:  Tumbleweed update bulan ini, September 2021
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 23 Agustus 2021, 4 minggu yang lalu, di *Snapshot* **20210817**. Dan *update* hari ini saya mendapatkan *Snapshot* **20210916**. Total paket yang diperbarui adalah 424 paket di-*upgrade*, 12 paket baru dan 10 paket dihapus, dengan total ukuran *download* sebesar **470,1 MiB**.

<!--more-->

Sebelum melakukan *update*, saya menghapus *lock* dari paket `patterns-microos-desktop-common` yang di bulan sebelumnya di-*lock* karena membawa banyak paket baru. Kali ini, tanpa me-*lock* paket tersebut, proses *update* sudah kembali normal.

Dan detail *update* bulan ini adalah seperti berikut:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 424 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 NetworkManager NetworkManager-branding-openSUSE aaa_base accountsservice ark attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bind-utils bluedevil5 bluez bluez-qt-imports bluez-qt-udev breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules chkstat compat-usrmerge-tools cpio cpp cpp11 dhcp dhcp-client diffutils dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 elfutils ffmpegthumbs fprintd fprintd-pam frameworkintegration-plugin fuse gio-branding-openSUSE git-core glib2-tools gmenudbusmenuproxy gpg2 grep grub2 grub2-i386-pc gstreamer-plugins-base gtk3-metatheme-breeze gwenview5 hwdata iproute2 irqbalance kactivities5-imports kactivitymanagerd kate kate-plugins kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 kmod knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kquickcharts krb5 kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kwalletd5 kwayland kwin5 layer-shell-qt5 libAppStreamQt2 libBasicUsageEnvironment1 libGLU1 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kipi32_0_0 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKScreenLocker5 libKSysGuardSystemStats1 libKWaylandServer5 libLLVM12 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Multimedia5 libQt5Network5 libQt5Positioning5 libQt5PrintSupport5 libQt5Sql5 libQt5Sql5-sqlite libQt5Test5 libQt5TextToSpeech5 libQt5WaylandClient5 libQt5Widgets5 libQt5Xml5 libQtQuick5 libSDL2-2_0-0 libUsageEnvironment3 libaom3 libappstream4 libasm1 libaudit1 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libblkid1 libbluetooth3 libbreezecommon5-5 libbtrfs0 libcairo-gobject2 libcairo2 libcrypt1 libcryptsetup12 libcurl4 libdav1d5 libdcerpc-binding0 libdcerpc0 libdolphinvcs5 libdw1 libeditorconfig0 libelf1 libell0 libepoxy0 libfdisk1 libfdk-aac2 libfprint-2-2 libfreebl3 libfuse2 libgbm1 libgcc_s1 libgcrypt20 libgdbm6 libgdbm_compat4 libgio-2_0-0 libglib-2_0-0 libglslang11 libgmodule-2_0-0 libgobject-2_0-0 libgomp1 libgpg-error0 libgroupsock30 libgstallocators-1_0-0 libgstapp-1_0-0 libgstaudio-1_0-0 libgstgl-1_0-0 libgstpbutils-1_0-0 libgstphotography-1_0-0 libgstriff-1_0-0 libgsttag-1_0-0 libgstvideo-1_0-0 libharfbuzz-subset0 libharfbuzz0 libibus-1_0-5 libixml11 libjpeg8 libjson-glib-1_0-0 libkaccounts2 libkdecorations2-5 libkdecorations2private8 libkerfuffle21 libkeyutils1 libkioarchive5 libkipi-data libkmod2 libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 libldap-2_4-2 libliveMedia97 libmm-glib0 libmount1 libmpg123-0 libncurses6 libndr-krb5pac0 libndr-nbt0 libndr-standard0 libndr1 libnetapi0 libnftables1 libnl-config libnl3-200 libnm0 libnuma1 libopenmpt0 libopenssl1_1 libp11-kit0 libpango-1_0-0 libphonon4qt5 libpipewire-0_3-0 libpkgconf3 libpolkit-qt5-1-1 libpoppler-qt5-1 libpostproc55_9 libpulse-mainloop-glib0 libpulse0 libpython3_8-1_0 libqt5-qdbus libqt5-qtpaths libqt5-qtwebengine libre2-9 librtmp1 libsamba-credentials1 libsamba-errors0 libsamba-hostconfig0 libsamba-passdb0 libsamba-util0 libsamdb0 libsasl2-3 libseccomp2 libsemanage-conf libsemanage2 libsensors4 libserd-0-0 libshaderc_shared1 libsmartcols1 libsmbclient0 libsmbconf0 libsmbldap2 libsoftokn3 libssh-config libssh4 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtevent-util0 libubsan1 libudev1 libupnp17 libuuid1 libuv1 libvlc5 libvlccore9 libvo-amrwbenc0 libvulkan1 libwbclient0 libx264-161 libx265-199 libxkbcommon-x11-0 libxkbcommon0 libxvidcore4 libzbar0 libzypp metatheme-breeze-common milou5 mobipocket mozilla-nss mozilla-nss-certs ncurses-utils nftables numactl obs-studio okular openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common p11-kit p11-kit-tools pam pam-config pam_unix-nis permissions permissions-config pinentry pkgconf pkgconf-m4 pkgconf-pkg-config plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit-kde-agent-5 powerdevil5 prison-qt5-imports pulseaudio pulseaudio-module-bluetooth pulseaudio-module-x11 pulseaudio-utils python3-bind python3-nftables python38 python38-base python38-gobject samba-libs samba-libs-python3 solid-imports sonnet spectacle suse-module-tools syntax-highlighting system-group-hardware system-group-kvm system-user-lp system-user-nobody system-user-srvGeoClue systemd systemd-sysvinit systemsettings5 sysuser-shadow terminfo-base typelib-1_0-NM-1_0 udev util-linux util-linux-systemd vlc vlc-noX vlc-qt xdg-desktop-portal-kde xembedsniproxy xen-libs xrdb xterm-bin zypper

The following product is going to be upgraded:
openSUSE Tumbleweed
  20210817-0 -> 20210916-0

The following 12 NEW packages are going to be installed:
  kernel-default-5.14.2-1.3 libIex-3_1-30 libIlmThread-3_1-30 libImath-3_1-29 libOpenEXR-3_1-30 libSPIRV-Tools-suse22 libcodec2-1_0 libmpdec3 libnsl3 libplacebo157 libpoppler112 v4l2loopback-kmp-default-0.12.5_k5.14.2_1-5.36

The following 10 packages are going to be REMOVED:
  libHalf-2_5-25 libIex-2_5-25 libIlmImf-2_5-25 libIlmThread-2_5-25 libImath-2_5-25 libSPIRV-Tools-suse21 libcodec2-0_9 libnsl2 libplacebo120 libpoppler111

The following package requires a system reboot:
  kernel-default-5.14.2-1.3

424 packages to upgrade, 12 new, 10 to remove.
Overall download size: 470.1 MiB. Already cached: 0 B. After the operation, additional 179.5 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* berikutnya adalah sekitar tanggal 17 Oktober 2021, 4 minggu dari sekarang.

