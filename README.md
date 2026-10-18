# LunaMusic updates

Official Android update downloads for LunaMusic Mobile and TV.

[Latest release](https://github.com/lunavibe07/LunaMusic-updates/releases/latest)

**0.3.12:** [Mobile APK](https://github.com/lunavibe07/LunaMusic-updates/releases/download/v0.3.12/LunaMusic-0.3.12-mobile-debug.apk) | [TV APK](https://github.com/lunavibe07/LunaMusic-updates/releases/download/v0.3.12/LunaMusic-0.3.12-tv-debug.apk)

Version 0.3.12 improves storage migration and conservative unused-download cleanup, reclaims installed update APK caches, uses a static update feed with retry backoff, and interrupts stalled TV transfers. Playback, offline downloads, queues, direct voice search and TV pairing are retained.

## Changes in 0.3.12

- **Less update storage:** opening the updated app removes cached APKs already installed and abandoned update partials, while preserving newer APKs awaiting installation.
- **Fewer GitHub API requests:** update checks use a public static feed with caching and retry backoff, retaining APK verification.
- **Safer download cleanup:** **Clean unused downloads** is available in both options menus and also runs after successful downloads. Only recognized completed files without library references are eligible; playing queues, active transfers/exports, resumable partials and unknown files are protected. Unreadable metadata stops cleanup.
- **Safer library migration:** compare full file contents and preserve conflicting originals; bound library/history metadata reads.
- **Stalled TV transfer handling:** stop uploads after 30 seconds without progress or 30 minutes in total. File exports respond to cancellation between chunks and clean only their own incomplete output.
- **Updated Android libraries:** retain Android 8+ and ARM64/ARM32/x86_64 support. The Music assistant remains removed; direct voice search remains available.

Both editions passed APK builds/lint and 112 unit tests each. Three update-feed tests and six Android storage integration tests passed. Both LDPlayer editions downloaded, verified and installed the public 0.3.12 update over 0.3.11; installed update caches were reclaimed. Physical TV transfer stalls and provider-specific export failures remain unverified.

## Choose and install

- Mobile APK: touch interface for phones/tablets.
- TV APK: landscape interface with D-pad navigation.
- Each APK includes ARM64, ARM32 and x86_64. Install as an update, keeping the existing app/data.

Starting with 0.3.9, open **App update** in LunaMusic's options menu. The app can check automatically when opened, download its matching edition and verify the checksum, package, newer version and signing identity. Android asks before installation; the app does not silently install updates.

This repository is public so no GitHub token or sign-in is needed in the app. The development repository remains private. Each release includes the application source ZIP and retained notices. See [source references](UPSTREAM_SOURCES.md) for pinned upstream sources and native build instructions. APKs contain GPL components and are not MIT-only. Supplied artwork retains its original permissions.

Do not uninstall to update: uninstalling can remove downloaded music and local history. Older app versions need this APK installed manually once before the in-app updater becomes available.
