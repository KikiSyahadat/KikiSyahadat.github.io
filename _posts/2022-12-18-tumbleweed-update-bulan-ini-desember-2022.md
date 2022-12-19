---
title:  Tumbleweed update bulan ini, Desember 2022
tags:
  - openSUSE
  - Tumbleweed
  - Update
---

*Update* sebelumnya saya lakukan pada tanggal 20 November 2022, 4 pekan yang lalu, di *Snapshot* **20221118**. Dan di *update* kali ini saya mendapatkan *Snapshot* **20221216**. Total paket yang diperbarui adalah: 425 paket *upgrade**, 3 paket *downgrade*, 19 paket baru dan 6 paket dihapus dengan total ukuran *download* sebesar **673,4 MiB**.

<!--more-->

Setelah melakukan *update* saya memasang paket `sudo`. Dan berikut adalah rincian *update* kali ini:

```
Loading repository data...
Reading installed packages...
Warning: You are about to do a distribution upgrade with all enabled repositories. Make sure these repositories are compatible before you continue. See 'man zypper' for more information about this command.
Computing distribution upgrade...

The following 425 packages are going to be upgraded:
  Mesa Mesa-dri Mesa-gallium Mesa-libEGL1 Mesa-libGL1 Mesa-libglapi0 Mesa-vulkan-device-select NetworkManager NetworkManager-branding-openSUSE NetworkManager-openvpn ark attica-qt5 baloo5-imports baloo5-kioslaves baloo5-widgets bash bash-sh bluedevil5 bluez bluez-qt-imports bluez-qt-udev breeze breeze5-cursors breeze5-decoration breeze5-icons breeze5-style btrfsprogs btrfsprogs-udev-rules busybox cpp12 cups-config dolphin dolphin-part dracut dracut-mkinitrd-deprecated drkonqi5 elfutils ffmpegthumbs filesystem firewalld frameworkintegration-plugin gawk gio-branding-openSUSE git-core glib2-tools glibc glibc-locale-base gmenudbusmenuproxy gpg2 grub2 grub2-i386-pc gtk3-data gtk3-metatheme-breeze gtk3-schema gtk3-tools gwenview5 hicolor-icon-theme hwdata iproute2 iputils iso-codes iso-codes-lang kactivities5-imports kactivitymanagerd kate kate-plugins kcmutils-imports kconf_update5 kdbusaddons-tools kde-cli-tools5 kde-gtk-config5 kdeclarative-components kded kdelibs4support kdialog kernel-firmware-bluetooth kernel-firmware-i915 kernel-firmware-iwlwifi kexec-tools kfilemetadata5 kglobalaccel5 khotkeys5 kinfocenter5 kinit kio kio-core kio-extras5 kirigami2 kitemmodels-imports kmenuedit5 knewstuff knewstuff-imports konsole konsole-part kpackage kpeople5 kpipewire-imports kquickcharts krb5 kscreen5 kscreenlocker kservice ksysguardsystemstats-data ksystemstats5 ktexteditor kwalletd5 kwayland kwin5 layer-shell-qt5 libBasicUsageEnvironment1 libFLAC12 libICE6 libIex-3_1-30 libIlmThread-3_1-30 libImath-3_1-29 libKF5Activities5 libKF5ActivitiesStats1 libKF5Archive5 libKF5Attica5 libKF5Auth5 libKF5AuthCore5 libKF5Baloo5 libKF5BalooEngine5 libKF5BluezQt6 libKF5Bookmarks5 libKF5CalendarEvents5 libKF5Codecs5 libKF5Completion5 libKF5ConfigCore5 libKF5ConfigGui5 libKF5ConfigQml5 libKF5ConfigWidgets5 libKF5CoreAddons5 libKF5Crash5 libKF5DBusAddons5 libKF5DNSSD5 libKF5Declarative5 libKF5DocTools5 libKF5GlobalAccel5 libKF5GlobalAccelPrivate5 libKF5GuiAddons5 libKF5Holidays5 libKF5I18n5 libKF5IconThemes5 libKF5IdleTime5 libKF5ItemModels5 libKF5ItemViews5 libKF5JS5 libKF5JSApi5 libKF5JobWidgets5 libKF5KCMUtils5 libKF5KCMUtilsCore5 libKF5KDELibs4Support5 libKF5KDcraw5 libKF5KExiv2-15_0_0 libKF5KHtml5 libKF5Kirigami2-5 libKF5ModemManagerQt6 libKF5NetworkManagerQt6 libKF5NewStuff5 libKF5NewStuffCore5 libKF5NewStuffWidgets5 libKF5Notifications5 libKF5NotifyConfig5 libKF5Parts5 libKF5Plasma5 libKF5Prison5 libKF5Pty5 libKF5Purpose5 libKF5PurposeWidgets5 libKF5QuickAddons5 libKF5Runner5 libKF5Screen7 libKF5Solid5 libKF5SonnetCore5 libKF5SonnetUi5 libKF5Style5 libKF5Su5 libKF5Syndication5 libKF5SyntaxHighlighting5 libKF5TextWidgets5 libKF5ThreadWeaver5 libKF5UnitConversion5 libKF5Wallet5 libKF5WidgetsAddons5 libKF5WindowSystem5 libKF5XmlGui5 libKPipeWire5 libKPipeWireRecord5 libKScreenLocker5 libKSysGuardSystemStats1 libLLVM15 libOpenEXR-3_1-30 libQt5Concurrent5 libQt5Core5 libQt5DBus5 libQt5Gui5 libQt5Network5 libQt5PrintSupport5 libQt5Sql5 libQt5Sql5-sqlite libQt5Test5 libQt5Widgets5 libQt5Xml5 libSDL2-2_0-0 libSvtAv1Enc1 libUsageEnvironment3 libXRes1 libXcomposite1 libXdamage1 libXdmcp6 libXpm4 libXrandr2 libXss1 libXv1 libXxf86dga1 libapparmor1 libasm1 libass9 libavahi-client3 libavahi-common3 libavcodec58_134 libavdevice58_13 libavfilter7_110 libavformat58_76 libavresample4_0 libavutil56_70 libbluetooth3 libbluray2 libbreezecommon5-5 libbtrfs0 libcaca0 libchromaprint1 libcrypt1 libcryptsetup12 libcups2 libdolphinvcs5 libdrm2 libdrm_amdgpu1 libdrm_intel1 libdrm_nouveau2 libdrm_radeon1 libduktape206 libdw1 libeconf0 libelf1 libell0 libexiv2-27 libexpat1 libfdk-aac2 libfreebl3 libgbm1 libgcc_s1 libgcrypt20 libgif7 libgio-2_0-0 libglib-2_0-0 libglvnd libgmodule-2_0-0 libgnutls30 libgobject-2_0-0 libgomp1 libgroupsock30 libgtk-3-0 libibus-1_0-5 libinput10 libixml11 libkaccounts2 libkdecorations2-5 libkdecorations2private9 libkerfuffle22 libkioarchive5 libkscreen2-plugin libksysguard5 libksysguard5-imports libkwalletbackend5-5 liblcms2-2 libldap2 libliveMedia107 libluajit-5_1-2 liblzma5 libmfx1 libminizip1 libmpc3 libmpfr6 libncurses6 libnghttp2-14 libnm0 libopenssl3 liborc-0_4-0 libpango-1_0-0 libpci3 libpcre2-16-0 libpcre2-8-0 libpipewire-0_3-0 libpng16-16 libpoppler-qt5-1 libpostproc55_9 libprocps8 libprotobuf-c1 libpulse-mainloop-glib0 libpulse0 libpython3_10-1_0 libqca-qt5-2 libqt5-qtwebengine librav1e0 librtmp1 libsasl2-3 libshaderc_shared1 libslang2 libsnapper6 libsoftokn3 libsolv-tools libsqlite3-0 libstdc++6 libswresample3_9 libswscale5_9 libsystemd0 libtag1 libubsan1 libudev1 libupnp17 libva-drm2 libva-wayland2 libva-x11-2 libva2 libvlc5 libvlccore9 libvo-amrwbenc0 libvulkan_intel libwireplumber-0_4-0 libx264-161 libx265-199 libxvidcore4 libz1 libzvbi0 libzypp metatheme-breeze-common milou5 mobipocket mozilla-nss mozilla-nss-certs ncurses-utils obs-studio okular openSUSE-release openSUSE-release-appliance-custom openssh-clients openssh-common openvpn otpclient pam pam-manpages pam_unix pciutils perl-Bootloader pipewire pipewire-alsa pipewire-modules-0_3 pipewire-pulseaudio pipewire-spa-plugins-0_2 pipewire-spa-tools pipewire-tools plasma-framework plasma-framework-components plasma-nm5 plasma-nm5-openvpn plasma5-addons plasma5-desktop plasma5-integration-plugin plasma5-pa plasma5-session plasma5-workspace plasma5-workspace-libs polkit-kde-agent-5 powerdevil5 prison-qt5-imports procps pulseaudio-setup pulseaudio-utils purpose python3-firewall python310-base qca-qt5 rpm samba-ad-dc-libs samba-client-libs samba-libs snapper solid-imports sonnet spectacle suse-module-tools syntax-highlighting syntax-highlighting-imports sysconfig sysconfig-netconfig systemd systemd-presets-common-SUSE systemd-rpm-macros systemsettings5 terminfo-base timezone typelib-1_0-NM-1_0 ucode-intel udev vlc vlc-noX vlc-qt wayland-utils wireplumber wireplumber-audio xdg-desktop-portal xdg-desktop-portal-kde xdm xembedsniproxy xen-libs xinit xorg-x11-server xorg-x11-server-Xvfb xprop xset xterm-bin xterm-resize xz

The following product is going to be upgraded:
openSUSE Tumbleweed
  20221118-0 -> 20221216-0

The following 3 packages are going to be downgraded:
  libX11-6 libX11-data libX11-xcb1

The following 19 NEW packages are going to be installed:
  kernel-default-6.0.12-1.1 libavcodec59 libavfilter8 libavformat59 libavutil57 libbrotlienc1 libglslang11 libhwy1 libjxl0_7 libplacebo229 libpoppler126 libpostproc56 libprotobuf-lite3_21_11 libre2-10 librist4 libswresample4 libswscale6 suse-module-tools-scriptlets v4l2loopback-kmp-default-0.12.7_k6.0.12_1-1.12

The following 6 packages are going to be REMOVED:
  libcfitsio9 libglslang11_12 libplacebo208 libpoppler125 libprotobuf-lite3_21_9 libre2-9

The following package requires a system reboot:
  kernel-default-6.0.12-1.1

425 packages to upgrade, 3 to downgrade, 19 new, 6 to remove.
Overall download size: 673.4 MiB. Already cached: 0 B. After the operation, additional 301.2 MiB will be used.

    Note: System reboot required.
Continue? [y/n/v/...? shows all options] (y): 
```

Jadwal *update* berikutnya adalah sekitar tanggal 22 Januari 2023 atau 5 pekan dari sekarang.

