---
title:  Tumbleweed update bulan ini, November 2022
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 16 Oktober 2022, 5 pekan yang lalu, di *Snapshot* **20221014**. Dan di *update* kali ini saya mendapatkan *Snapshot* **20221118**. Total paket yang diperbarui adalah: 469 paket *upgrade*, 16 paket baru dan 9 paket dihapus, dengan total ukuran *download* sebesar **686,5 MiB**.

<!--more-->

Sebelum melakukan *update* saya menghapus paket `MozillaFirefox` dan `MozillaThunderbird`. Dan setelahnya, saya memasang paket `libdbus-glib-1-2`. Karena tanpa ini, **Firefox** dan **Thunderbird** yang saya *download* dari *website* resmi masing-masing tidak bisa jalan.

Setelah *update* saya mendapatkan masalah pada *layout keyboard* yang tidak muncul dan tidak bisa diubah. Saya belum mencari tahu masalahnya dari mana dan penyelesaiannya seperti apa, karena saat ini saya belum terlalu butuh ini.

Berikut adalah rincian *update* kali ini:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 469 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 Mesa-vulkan-device-select NetworkManager NetworkManager-branding-openSUSE alts ark attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bash bash-sh bluedevil5 bluez bluez-qt-imports bluez-qt-udev boost-license1_80_0 breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules busybox coreutils cpp12 dbus-1 dbus-1-common dbus-1-daemon dbus-1-tools dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 elfutils ffmpegthumbs firewalld fontconfig frameworkintegration-plugin gdk-pixbuf-query-loaders gettext-runtime gio-branding-openSUSE git-core glib2-tools glibc glibc-locale-base gmenudbusmenuproxy gpg2 grub2 grub2-i386-pc gstreamer gstreamer-plugins-base gtk3-metatheme-breeze gwenview5 hwdata iio-sensor-proxy iproute2 irqbalance kactivities5-imports kactivitymanagerd kate kate-plugins kcmutils-imports kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kexec-tools kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kpipewire-imports kquickcharts krb5 kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kuserfeedback-imports kwalletd5 kwayland kwin5 layer-shell-qt5 libIex-3_1-30 libIlmThread-3_1-30 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigQml5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KCMUtilsCore5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5NewStuffWidgets5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5Syndication5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5UnitConversion5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKPipeWire5 libKPipeWireRecord5 libKScreenLocker5 libKSysGuardSystemStats1 libKUserFeedbackCore1 libKUserFeedbackWidgets1 libLLVM15 libOpenEXR-3_1-30 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Multimedia5 libQt5Network5 libQt5Positioning5 libQt5PrintSupport5 libQt5QuickControls2-5 libQt5QuickTemplates2-5 libQt5Sensors5 libQt5Sql5 libQt5Sql5-sqlite libQt5Svg5 libQt5Test5 libQt5TextToSpeech5 libQt5VirtualKeyboard5 libQt5WaylandClient5 libQt5WebChannel5 libQt5WebChannel5-imports libQt5Widgets5 libQt5X11Extras5 libQt5Xml5 libQtQuick5 libSDL2-2_0-0 libSvtAv1Enc1 libX11-6 libX11-data libX11-xcb1 libXext6 libXft2 libXinerama1 libXmu6 libXmuu1 libXrender1 libaa1 libalternatives1 libasm1 libasound2 libatk-1_0-0 libatk-bridge-2_0-0 libatspi0 libaugeas0 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libbluetooth3 libboost_thread1_80_0 libbreezecommon5-5 libbtrfs0 libcrypt1 libcurl4 libdbus-1-3 libdevmapper1_03 libdolphinvcs5 libdrm2 libdrm_amdgpu1 libdrm_intel1 libdrm_nouveau2 libdrm_radeon1 libdw1 libeconf0 libelf1 libepoxy0 libexiv2-27 libexpat1 libexslt0 libfa1 libfdk-aac2 libffi8 libfontconfig1 libfreebl3 libgbm1 libgcc_s1 libgdk_pixbuf-2_0-0 libgio-2_0-0 libglib-2_0-0 libgmodule-2_0-0 libgnutls30 libgobject-2_0-0 libgomp1 libgpg-error0 libgpgme11 libgpgmepp6 libgstallocators-1_0-0 libgstapp-1_0-0 libgstaudio-1_0-0 libgstgl-1_0-0 libgstpbutils-1_0-0 libgstphotography-1_0-0 libgstreamer-1_0-0 libgstriff-1_0-0 libgsttag-1_0-0 libgstvideo-1_0-0 libharfbuzz-subset0 libharfbuzz0 libidn2-0 libkaccounts2 libkdecorations2-5 libkdecorations2private9 libkerfuffle22 libkioarchive5 libksba8 libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 liblcms2-2 libldap2 liblilv-0-0 libmad0 libmbedcrypto7 libmbedtls14 libmbedx509-1 libmfx-gen1_2 libmfx1 libmpg123-0 libmysofa1 libncurses6 libnftnl11 libnm0 libopenssl1_1 libopenssl3 libpciaccess0 libpipewire-0_3-0 libpixman-1-0 libpkcs11-helper1 libpolkit-agent-1-0 libpolkit-gobject-1-0 libpostproc55_9 libprotobuf-c1 libpsl5 libpulse-mainloop-glib0 libpulse0 libpython3_10-1_0 libqalculate22 libqca-qt5-2 libqt5-qdbus libqt5-qtgraphicaleffects libqt5-qtimageformats libqt5-qtpaths libqt5-qtquickcontrols libqt5-qtquickcontrols2 libqt5-qtvirtualkeyboard libqt5-qtwebengine libreadline8 librtmp1 libshaderc_shared1 libslp1 libsoftokn3 libsord-0-0 libsqlite3-0 libstdc++6 libsubid4 libswresample3_9 libswscale5_9 libsystemd0 libtextstyle0 libtiff5 libubsan1 libudev1 libva-drm2 libva-wayland2 libva-x11-2 libva2 libvlc5 libvlccore9 libvmaf1 libvo-amrwbenc0 libvulkan1 libvulkan_intel libwireplumber-0_4-0 libx264-161 libx265-199 libxcb-cursor0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-render-util0 libxkbfile1 libxml2-2 libxshmfence1 libxslt1 libxvidcore4 libzck1 libzypp login_defs metatheme-breeze-common milou5 mobipocket mozilla-nspr mozilla-nss mozilla-nss-certs ncurses-utils netcfg obs-studio okular openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common pam pam-config pam-manpages pam_unix pipewire pipewire-alsa pipewire-modules-0_3 pipewire-pulseaudio pipewire-spa-plugins-0_2 pipewire-spa-tools pipewire-tools pkcs11-helper plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-addons plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit polkit-kde-agent-5 powerdevil5 prison-qt5-imports pulseaudio-setup purpose python3-firewall python310-base qca-qt5 qtdeclarative-imports-provides-qt5 rpm rsync samba-client-libs sddm sddm-branding-upstream sed sessreg sg3_utils shadow solid-imports sonnet spectacle suse-module-tools syntax-highlighting syntax-highlighting-imports system-user-srvGeoClue systemd systemsettings5 terminfo-base timezone typelib-1_0-NM-1_0 udev vlc vlc-noX vlc-qt vulkan-tools wireplumber wireplumber-audio xdg-desktop-portal-kde xembedsniproxy xkeyboard-config xorg-x11-server xorg-x11-server-Xvfb xsetroot xterm-bin xterm-resize zypper

The following product is going to be upgraded:
openSUSE Tumbleweed
  20221014-0 -> 20221118-0

The following 16 NEW packages are going to be installed:
  kernel-default-6.0.8-1.1 libSPIRV-Tools-2022_4 libbpf1 libcamera-base0_0_1 libcamera0_0_1 libglslang11_12 libicu72 libicu72-ledata libluajit-5_1-2 libprotobuf-lite3_21_9 libsgutils2-1_48-2 libunistring5 pulseaudio-utils samba-ad-dc-libs samba-libs v4l2loopback-kmp-default-0.12.7_k6.0.8_1-1.10

The following 9 packages are going to be REMOVED:
  libSPIRV-Tools-2022_3 libbpf0 libcamera-suse7 libglslang11 libicu71 libicu71-ledata libprotobuf-lite3_21_6 libsgutils2-1_47-2 libunistring2

The following package requires a system reboot:
  kernel-default-6.0.8-1.1

469 packages to upgrade, 16 new, 9 to remove.
Overall download size: 686.5 MiB. Already cached: 0 B. After the operation, additional 541.1 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* berikutnya adalah sekitar tanggal 18 Desember 2022, 4 pekan dari sekarang.

---

**Update 22 November 2022**: Masalah pada *layout keyboard* ternyata hanya perlu menghapus dan menambahkan ulang saja di **System Settings** > **Input Devices** > **Keyboard** > **Layout** > **Configure layouts**.

