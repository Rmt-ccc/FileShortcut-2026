# https://release-assets.githubusercontent.com/github-production-release-asset/1366888944/d93274bc-629b-4576-bbad-29250b33ed42?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-10-27T13%3A57%3A05Z&rscd=attachment%3B+filename%3Dapp-debug.apk&rsct=application%2Fvnd.android.package-archive&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-10-27T12%3A56%3A46Z&ske=2026-10-27T13%3A57%3A05Z&sks=b&skv=2018-11-09&sig=yiRKUUTy7ZiKyRkXmwGU5vwGvX9Vxv1LJ08P%2BXEfqpo%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc5MzEwNjI0NSwibmJmIjoxNzkzMTA1OTQ1LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.oeDu3Tz7WD97fcr2hSWQQwoessOHQXh7j6wqtEhL1lw&response-content-disposition=attachment%3B%20filename%3Dapp-debug.apk&response-content-type=application%2Fvnd.android.package-archive

# FileShortcut 2026 [![Build APK](https://github.com/75py/FileShortcut/actions/workflows/build.yml/badge.svg)](https://github.com/75py/FileShortcut/actions/workflows/build.yml)

Create shortcuts to open your files!

## ⚠️ Unofficial fork

This is an **unofficial**, community-maintained fork of the original [FileShortcut](https://github.com/75py/FileShortcut) by [75py](https://github.com/75py). All credit for the original app, design, and concept goes to the original author. This fork is not endorsed by or affiliated with 75py.

This fork exists to keep the app buildable on modern Android toolchains, since the original project (last released around 2018) no longer builds due to dependencies and services that have since been discontinued (e.g. JCenter).

## Why this fork exists

I was putting together a collection of handy Android apps and thought it would be nice to be able to add files to the home screen, the way you can drop shortcuts on a computer desktop. Searching for something open source on GitHub, I happened to come across this project.

When I tried to just download an APK from the Releases page, I found that no APK had ever been published there, and the last release was old enough that it no longer runs on current Android versions. So, instead of just building it once for myself, I decided to modernize it properly as an unofficial update so it keeps building going forward.

### What changed in this fork

- Updated to a modern toolchain: Gradle 8.7, Android Gradle Plugin 8.5.2, Kotlin 2.0.21
- Removed dependency on JCenter (shut down in 2024); all dependencies now resolve from Google's Maven and Maven Central
- Migrated from the old `com.android.support` libraries to AndroidX
- Removed Kodein (dependency injection library, no longer maintained) in favor of plain manual dependency management
- Removed PermissionsDispatcher in favor of the modern Activity Result API
- Raised `minSdkVersion` from 19 to 21 (required by current AndroidX libraries)
- Renamed the app to "FileShortcut 2026" to distinguish it from the original, still-listed Play Store app

No functional changes were intentionally made beyond what was necessary to get the app building and running on current Android versions.

## Download

This fork is **not** published on the Google Play Store or F-Droid. The only official distribution channel is this repository's [Releases](https://github.com/75py/FileShortcut/releases) page (or the `app-debug-apk` artifact from the [Actions](https://github.com/75py/FileShortcut/actions) tab for the latest build).

Every build is produced automatically by [GitHub Actions](https://github.com/75py/FileShortcut/actions), and each APK is automatically submitted to [VirusTotal](https://www.virustotal.com/gui/) for a malware scan as part of that same workflow. Open a workflow run and check its summary for a direct link to that build's scan report.

If you'd rather not trust a pre-built APK from anyone, you don't have to: **fork this repository and run the "Build APK" GitHub Action yourself.** It will build the APK from source in front of you and, once you add your own VirusTotal API key as a repository secret (`VT_API_KEY`), it will also scan that exact build and give you a direct link to its own VirusTotal report — no computer required, this works entirely from GitHub's website or app.

**Before installing an APK from any source, including this one, please verify it yourself** — check the scan report above, or scan the file yourself at [virustotal.com](https://www.virustotal.com/gui/) before installing. Only install APKs from sources you trust.

## Disclaimer

This software is provided "as is", without warranty of any kind. The maintainer(s) of this fork are not responsible for any damage, data loss, or other issues resulting from its use. Use at your own risk.

## Original project

- Original repository: https://github.com/75py/FileShortcut
- Original author: [75py](https://github.com/75py)

## releases
https://github.com/Rmt-ccc/FileShortcut/releases/tag/v1.0.0

