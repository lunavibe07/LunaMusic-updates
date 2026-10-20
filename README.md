# LunaMusic updates

Official Android update downloads for LunaMusic Mobile and TV.

[Latest release](https://github.com/lunavibe07/LunaMusic-updates/releases/latest)

**0.3.14:** [Mobile APK](https://github.com/lunavibe07/LunaMusic-updates/releases/download/v0.3.14/LunaMusic-0.3.14-mobile-debug.apk) | [TV APK](https://github.com/lunavibe07/LunaMusic-updates/releases/download/v0.3.14/LunaMusic-0.3.14-tv-debug.apk)

Version 0.3.14 (versionCode 17) adds English/Vietnamese language selection, three illustrated themes, a YouTube-only Mobile drawer and a larger launcher logo. Both APKs are signed with the existing certificate and install over 0.3.13 while preserving app data.

## Changes in 0.3.14

- Select English or Vietnamese on Mobile and TV.
- Choose Synthwave Neon, Forest Night or Rose Quartz theme artwork.
- Navigate Mobile with a YouTube-only drawer and quick navigation bar.
- See the enlarged LunaMusic launcher logo.

Both editions passed APK assembly and lint plus 112 unit tests each. All 3 update-feed tests passed. Both editions installed and opened on LDPlayer 07/05. The APK checksums and the shared signing identity are included/verified in the release assets.

## Choose and install

- Mobile APK: touch interface for phones/tablets.
- TV APK: landscape interface with D-pad navigation.
- Each APK includes ARM64, ARM32 and x86_64. Install as an update, keeping the existing app/data.

Starting with 0.3.9, open **App update** in LunaMusic's options menu. The app can check automatically when opened, download its matching edition and verify the checksum, package, newer version and signing identity. Android asks before installation; the app does not silently install updates.

This repository is public so no GitHub token or sign-in is needed in the app. The development repository remains private. Each release includes the application source ZIP and retained notices. See [source references](UPSTREAM_SOURCES.md) for pinned upstream sources and native build instructions. APKs contain GPL components and are not MIT-only. Supplied artwork retains its original permissions.

Do not uninstall to update: uninstalling can remove downloaded music and local history. Older app versions need this APK installed manually once before the in-app updater becomes available.
