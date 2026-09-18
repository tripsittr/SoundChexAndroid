# SoundChex for Android

The native Android client for a self-hosted SoundChex library — one codebase for
**phone, tablet, Android TV, Google TV, and Amazon Fire TV**, all of which are
Android and share this Kotlin/Gradle build.

It talks to the SoundChex server's JSON API (`/api/v1/*`) — the same API the
native iOS app uses (profiles, token auth, streaming, progress, search,
playlists, admin). The media stays on the user's own server; this is a window
onto it.

## Why one repo for five form factors

Android TV and Google TV run Android TV; **Amazon Fire OS is a fork of Android**,
so Fire TV apps are Android apps. All five build from this one Kotlin project and
differ only in **leanback/TV UI vs. touch UI** and in **distribution** (Play
Store, Amazon Appstore, sideload). Splitting them would duplicate the
networking, models, and playback layers for no gain.

## Planned stack

- **Kotlin + Jetpack Compose** (Compose for the phone/tablet UI, **Compose for
  TV / Leanback** for the 10-foot UI).
- **Media3 (ExoPlayer)** for playback, background audio, and PiP.
- Same API surface as `SoundChexiOS`; a shared networking/model layer, TV and
  handset presentation on top.

## Status

Scaffold only — see [Documentation & Planning/Status.md](Documentation%20&%20Planning/Status.md)
and [Roadmap.md](Documentation%20&%20Planning/Roadmap.md). No app code yet.

## Licence

**Dual-licensed** — **AGPL-3.0-or-later** by default (see [LICENSE](LICENSE)), or
a **commercial licence** for those who can't/won't comply with the AGPL. Full
terms, the contributor agreement, and the commercial option live in the main
repo: [LICENSING.md](https://github.com/tripsittr/SoundChex/blob/main/LICENSING.md)
(contact `licensing@soundchex.app`). AGPL §13: a modified, network-hosted build
must offer its users the corresponding source.