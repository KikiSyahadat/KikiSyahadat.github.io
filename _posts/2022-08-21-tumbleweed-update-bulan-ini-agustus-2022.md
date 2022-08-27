---
title:  Tumbleweed update bulan ini, Agustus 2022
tags:
  - openSUSE
  - PipeWire
  - PulseAudio
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 17 Juli 2022, 5 pekan lalu, di *Snapshot* **20220714**. Dan di *update* kali ini saya mendapatkan *Snapshot* **20220819**. Total paket yang diperbarui adalah: 399 paket *upgrade*, 1 paket *downgrade*, 9 paket baru dan 5 paket dihapus, dengan total ukuran *download* sebesar **555.5 MiB**.

<!--more-->

Di antara *update* sebelumnya dengan *update* kali ini saya mengganti **PulseAudio** dengan **PipeWire** dan melengkapinya dengan `pipewire-alsa`, karena untuk Tumbleweed instalasi baru sekarang menggunakan **PipeWire**, sedangkan untuk instalasi lama harus melakukannya secara manual.

Berikut adalah rincian *update* kali ini:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 399 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 NetworkManager NetworkManager-branding-openSUSE aaa_base accountsservice ark attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bind-utils bluez-qt-imports breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules busybox chkstat coreutils cpp12 cups-config dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 elfutils ffmpegthumbs file file-magic firewalld frameworkintegration-plugin gdk-pixbuf-query-loaders git-core glibc glibc-locale-base gmenudbusmenuproxy gpg2 grep grub2 grub2-i386-pc gtk3-data gtk3-metatheme-breeze gtk3-schema gtk3-tools gwenview5 iio-sensor-proxy iproute2 iptables irqbalance iso-codes iso-codes-lang kactivities5-imports kactivitymanagerd kate kate-plugins kcmutils-imports kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kexec-tools kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kquickcharts kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kwalletd5 kwayland kwin5 layer-shell-qt5 less libBasicUsageEnvironment1 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigQml5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KCMUtilsCore5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5NewStuffWidgets5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5Syndication5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5UnitConversion5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKScreenLocker5 libKSysGuardSystemStats1 libLLVM14 libSvtAv1Enc1 libUsageEnvironment3 libapparmor1 libasm1 libasound2 libaugeas0 libavahi-client3 libavahi-common3 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libblkid1 libbluetooth3 libbluray2 libbpf0 libbreezecommon5-5 libbtrfs0 libcap2 libcodec2-1_0 libcups2 libcurl4 libdmtx0 libdolphinvcs5 libdrm2 libdrm_amdgpu1 libdrm_intel1 libdrm_nouveau2 libdrm_radeon1 libdw1 libeditorconfig0 libelf1 libfa1 libfdisk1 libfdk-aac2 libfreebl3 libgbm1 libgcc_s1 libgcrypt20 libgdk_pixbuf-2_0-0 libglvnd libgnutls30 libgomp1 libgroupsock30 libgsm1 libgtk-3-0 libharfbuzz-subset0 libharfbuzz0 libhogweed6 libip4tc2 libip6tc2 libisl23 libixml11 libjpeg8 libkaccounts2 libkdecorations2-5 libkdecorations2private9 libkerfuffle22 libkioarchive5 libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 libldap2 libldb2 liblirc_client0 libliveMedia107 liblz4-1 liblzma5 libmagic1 libmount1 libmpg123-0 libncurses6 libnettle8 libnfs14 libnftables1 libnftnl11 libnghttp2-14 libnm0 libnotify4 libopenal1 libopenjp2-7 libpackagekitqt5-1 libpango-1_0-0 libpcre2-16-0 libpcre2-8-0 libpipewire-0_3-0 libpolkit-agent-1-0 libpolkit-gobject-1-0 libpoppler-qt5-1 libpostproc55_9 libprotobuf-c1 libpulse-mainloop-glib0 libpulse0 libpython3_10-1_0 libqt5-qtwebengine librtmp1 librubberband2 libselinux1 libshaderc_shared1 libsmartcols1 libsnapper6 libsoftokn3 libsord-0-0 libsqlite3-0 libstdc++6 libswresample3_9 libswscale5_9 libtiff5 libubsan1 libupnp17 libupower-glib3 libuuid1 libuv1 libvlc5 libvlccore9 libvo-amrwbenc0 libvpx7 libwacom-data libwacom9 libwebp7 libwebpdemux2 libwebpmux3 libwireplumber-0_4-0 libx264-161 libx265-199 libxcvt0 libxmlb2 libxtables12 libxvidcore4 libyajl2 libzmq5 libzypp metatheme-breeze-common milou5 mobipocket mozilla-nspr mozilla-nss mozilla-nss-certs ncurses-utils nftables obs-studio okular openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common otpclient perl perl-base permissions-config phonon4qt5-backend-vlc pipewire pipewire-alsa pipewire-modules-0_3 pipewire-pulseaudio pipewire-spa-plugins-0_2 pipewire-spa-tools pipewire-tools plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-addons plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit polkit-kde-agent-5 powerdevil5 prison-qt5-imports pulseaudio-setup purpose python3-firewall python3-nftables python310-base python310-gobject rpm rsync samba-client-libs snapper solid-imports sonnet spectacle suse-module-tools syntax-highlighting syntax-highlighting-imports sysconfig sysconfig-netconfig systemsettings5 terminfo-base timezone typelib-1_0-NM-1_0 ucode-intel upower util-linux util-linux-systemd vlc vlc-noX vlc-qt vulkan-tools wireplumber wireplumber-audio xdg-desktop-portal xdg-desktop-portal-kde xembedsniproxy xen-libs xorg-x11-server xorg-x11-server-Xvfb xtables-plugins xz zypper

The following product is going to be upgraded:
openSUSE Tumbleweed
  20220714-0 -> 20220819-0

The following package is going to be downgraded:
  permissions

The following 9 NEW packages are going to be installed:
  aaa_base-extras boost-license1_80_0 kernel-default-5.19.1-1.1 libboost_thread1_80_0 libplacebo208 libpoppler123 libprotobuf-lite3_21_5 pkexec v4l2loopback-kmp-default-0.12.5_k5.19.1_1-6.22

The following 5 packages are going to be REMOVED:
  boost-license1_79_0 libboost_thread1_79_0 libplacebo192 libpoppler122 libprotobuf-lite32

The following package requires a system reboot:
  kernel-default-5.19.1-1.1

399 packages to upgrade, 1 to downgrade, 9 new, 5 to remove.
Overall download size: 555.5 MiB. Already cached: 0 B. After the operation, additional 284.9 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* berikutnya adalah sekitar tanggal 18 September 2022, 4 pekan dari sekarang.

