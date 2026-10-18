# Release source references

The public LunaMusic-updates releases provide the application source ZIP for each APK build, retained notices and references to the pinned youtubedl-android source archive. The main development repository remains private. The application source ZIP includes the Gradle wrapper, dependency versions, Android source, resources and build instructions. Signing keys, local tools and private task notes are excluded.

## youtubedl-android 0.18.1

The Maven `library`, `common` and `ffmpeg` modules declare GPL-3.0. Upstream tag `0.18.1` resolves to commit `864791ae478e5e32194722337286790829c0a689`:

- [Pinned source archive](https://github.com/yausername/youtubedl-android/archive/864791ae478e5e32194722337286790829c0a689.zip)
- [FFmpeg build instructions](https://github.com/yausername/youtubedl-android/blob/864791ae478e5e32194722337286790829c0a689/BUILD_FFMPEG.md)
- [Python build instructions](https://github.com/yausername/youtubedl-android/blob/864791ae478e5e32194722337286790829c0a689/BUILD_PYTHON.md)

The archive retains upstream source, packaged runtime assets and their existing notices. The upstream build notes reference Termux packages for FFmpeg, Python and their dependencies; consult those notes and the embedded component licenses when rebuilding or redistributing native components. This document does not assert that the application ZIP alone contains every upstream native dependency's corresponding source.

## Bundled yt-dlp

The checked-in zipapp reports version `2026.08.19`, release commit `594bd50c2c78ac432f81600d309fdc4e0a92d82c` in `yt_dlp/version.py`. Its SHA-256 is `1fa6733c37ea6fb51c99ad8fe785e7b7e5f3246c9b980230329d4fb72ed8d4d6`.

- [Pinned yt-dlp source](https://github.com/yt-dlp/yt-dlp/archive/594bd50c2c78ac432f81600d309fdc4e0a92d82c.zip)

The application can update this executable on-device from the stable upstream channel, so an updated device may use a different upstream version than the original APK.

## Other dependencies and supplied assets

AndroidX/Media3, Kotlin and coroutines retain their upstream Apache-2.0 terms. Exact Maven coordinates are in `app/build.gradle.kts` and transitive artifacts are resolved by Gradle. Original application code retains its MIT grant; complete APKs are not MIT-only. Supplied artwork retains its existing terms and provenance in `branding/theme-reference/SOURCE.md`. See `THIRD_PARTY_NOTICES.md` and `THIRD_PARTY_youtubedl.txt`.
