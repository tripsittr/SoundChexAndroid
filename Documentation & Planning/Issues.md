# Issues — SoundChex for Android

Everything tracked for the Android client (phone/tablet + Android TV + Google TV
+ Fire TV). `A-NN` numbering. Sections run **In progress → Open → Deferred →
Done**; nothing is deleted.

## In progress

_(none — scaffold only)_

## Open

| ID | What | Notes |
|----|------|-------|
| A-01 | Project scaffold | Kotlin + Gradle + Jetpack Compose project; min SDK, target SDK, module layout (shared core + handset UI + TV UI). Builds an empty app on device/emulator. |
| A-02 | API client + auth | Port the `/api/v1/*` client: profile picker + PIN, token auth, device name. Mirror `SoundChexiOS` APIClient. |
| A-03 | Library browse + search | Music/movies/shows/books from `/api/v1/library`; the local catalogue mirror + delta sync; search. |
| A-04 | Playback (Media3/ExoPlayer) | Token-authed streaming (auth header on the data source), background audio, lock-screen/notification controls, resume, PiP for video. |
| A-05 | Downloads + offline | Background downloads to app storage, offline browse, "download all" gated on free space — parity with iOS 0.3.0. |
| A-06 | Playlists | Create/edit/reorder/cover, parity with iOS 0.4.0 and the server playlist API. |
| A-07 | Admin panel | Dashboard, item edit, profile management, scan — parity with iOS. |
| A-08 | TV (10-foot) UI | Compose for TV / Leanback: D-pad focus, rows/cards, now-playing, TV-safe areas. Shares the core with the handset UI. |
| A-09 | Distribution | Play Store (phone/tablet/Android TV/Google TV) + Amazon Appstore (Fire TV) + sideload. Signing, listings, per-store form-factor targeting. |
| A-10 | Android Auto | Your library on the car dashboard via Android Auto's media interface (`MediaBrowserService` / Media3 `MediaLibraryService` browse tree + playback). A must-have; the Media3 playback core (A-04) is the foundation. |
| A-11 | Chromecast + AirPlay (sender) | Cast the current playback OUT to a Chromecast / Google TV (Google Cast SDK sender + a media receiver) and to AirPlay devices where reachable. A must-have. |

## Deferred

_(none yet)_

## Done

| ID | What | When | Notes |
|----|------|------|-------|
| A-00 | Repo + licence + docs | 2026-09-17 | Scaffold: README, AGPLv3 LICENSE, planning docs. |
