# Roadmap — SoundChex for Android

One Kotlin/Compose codebase, five form factors (phone, tablet, Android TV, Google
TV, Fire TV). Phases ship in order; each is usable before the next starts.

## Phase 1 — Foundation (A-01, A-02)
Kotlin/Compose project scaffold; API client + token auth (profile picker, PIN).
**Done when:** the app signs in against a real server and holds a token.

## Phase 2 — Browse & play (A-03, A-04)
Library browse + search + local catalogue mirror; Media3/ExoPlayer playback with
background audio, notification controls, resume, and video PiP.
**Done when:** you can browse the library and play music and video on a phone.

## Phase 3 — Offline & playlists (A-05, A-06)
Downloads + offline browse ("download all" gated on space); full playlist
create/edit/reorder/cover. **Done when:** parity with iOS 0.3–0.4.

## Phase 4 — TV UI (A-08)
Compose-for-TV 10-foot UI (D-pad focus, rows, safe areas) sharing the core.
**Done when:** the same build runs well on an Android TV / Fire TV device.

## Phase 5 — Admin & distribution (A-07, A-09)
Admin panel parity; Play Store + Amazon Appstore listings and signing.
**Done when:** installable from the stores on all five form factors.

## Later
Cast/second-screen, TV-specific niceties (screensaver, voice), Wear OS if it ever
makes sense.
