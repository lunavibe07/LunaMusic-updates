# License scope and third-party notices

## Original LunaMusic code

Original LunaMusic application code and project documentation owned by lunavibe07 are licensed under the [MIT License](LICENSE), copyright 2026 lunavibe07.

The MIT grant applies only to material whose copyright holder can grant it. It does not replace upstream licenses, third-party copyright notices, bundled executable/runtime licenses or separately licensed artwork. Third-party material retains its own terms even when it appears in this repository or inside an APK.

## Dependencies and bundled components

| Component | License information |
| --- | --- |
| youtubedl-android `library`, `common` and `ffmpeg` modules, version 0.18.1 | Their Maven POMs declare GPL-3.0. Preserve [the existing GPL notice](THIRD_PARTY_youtubedl.txt) and applicable upstream notices/source obligations. |
| AndroidX / Media3 | Apache-2.0; retain the licenses/notices supplied by the dependencies. |
| Kotlin / kotlinx.coroutines | Apache-2.0; retain the licenses/notices supplied by the dependencies. |
| Bundled yt-dlp zipapp, Python runtime, FFmpeg and their embedded components | Retain their upstream component licenses and notices. The MIT license of the app does not relicense these binaries or their contents. |
| Third-party or supplied artwork | Retains its applicable copyright and permissions unless its owner separately grants a license. |

This table describes scope and known direct dependencies; it is not an exhaustive inventory of every transitive or native component.

## APK distribution

MIT is compatible with GPL use, but it does not remove GPL obligations from a combined distribution. LunaMusic currently links GPL-3.0 youtubedl-android modules. Distributing an APK containing those modules must comply with their applicable GPL terms, including corresponding-source and notice requirements for the combined work. Do not describe the complete APK and all bundled components as MIT-only.

The original app files can retain their MIT grant while the combined distribution follows the applicable GPL terms. Adding this LICENSE does not retroactively change notices or licenses attached to previously published artifacts.

References:

- [MIT license text — Open Source Initiative](https://opensource.org/license/mit)
- [GNU guidance on GPL libraries](https://www.gnu.org/licenses/gpl-faq.en.html#IfLibraryIsGPL)
- [GNU license compatibility guidance](https://www.gnu.org/licenses/license-compatibility.en.html)
- [youtubedl-android upstream](https://github.com/yausername/youtubedl-android)

## User-supplied appearance reference

The four `app/src/main/res/drawable/theme_*.webp` scenes were supplied through the user's local AI Project OS reference page. Their original permissions remain applicable; an independent upstream artwork license has not been supplied or verified. They are excluded from the original-code MIT grant. Source paths and checksums are recorded in [the theme reference note](branding/theme-reference/SOURCE.md). The native palette implementation adapts the five user-selected color schemes; it does not embed the reference application's code or connect to its local server.
