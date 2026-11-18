# RitxxShh

An Android companion for Spotify. RitxxShh is a personal, rebranded fork of [Hush by coldMEW](https://github.com/coldMEW/Hush), which detects Spotify ad breaks and skips or mutes them using Android's supported debugging and media controls.

## RitxxShh details

- App name: **RitxxShh**
- Version: **1.1**
- Developer: **Rithik**
- Project and update releases: [github.com/ken-ritxx/ritxxshh](https://github.com/ken-ritxx/ritxxshh)
- Android package: `com.ritxx.ritxxshh`

RitxxShh checks the latest release in this repository. For in-app updates, publish a release with a newer version and attach a release APK signed with the same private signing key used for the installed build. Keep that key private and backed up; builds signed with another key cannot update the installed app.

## Features inherited from Hush

- Detects Spotify ad breaks and can skip or mute them.
- Optional Spotify-only DNS filtering.
- Setup using Wireless debugging, Shizuku, or root.
- Sleep timer, Android Auto options, and recent activity.
- No account or analytics service.

## Build

The Android project is in `android/` and uses Gradle with Java 17. Debug builds can be built with the included Gradle wrapper. Release builds need a signing properties file outside the repository at `~/.gradle/ritxxshh-signing.properties`, or a file path in `RITXXSHH_SIGNING`.

The signing properties contain `storeFile`, `storePassword`, `keyAlias`, and `keyPassword`. Do not commit that file or the keystore to GitHub.

## Upstream credit and license

RitxxShh is derived from [coldMEW/Hush](https://github.com/coldMEW/Hush). The upstream project and its contributors retain their original authorship. This fork changes the branding, app identity, version, and update source. The code remains under the [GNU General Public License v3.0](LICENSE); distributed modified builds must comply with that license and include the corresponding source.

RitxxShh is an independent project and is not affiliated with or endorsed by Spotify AB. Spotify is a trademark of Spotify AB. Using ad-skipping software may conflict with Spotify's terms; use at your own discretion.
