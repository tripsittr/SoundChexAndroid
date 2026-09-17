# Status — SoundChex for Android

**Scaffold.** Repo created 17 Sep 2026 with README, LICENSE (AGPLv3),
`.gitignore`, and this planning set. **No app code yet.**

## What exists

- Repository + licence + docs only.

## What's next

The first real step is IOS-parity groundwork — see
[Roadmap.md](Roadmap.md) and [Issues.md](Issues.md). In short: scaffold a
Kotlin/Compose project, then build auth → browse → playback against the existing
`/api/v1/*` API (already built for iOS), then add the TV (leanback) UI, then
per-store distribution (Play, Amazon Appstore).

## Shared context

- The server API is in the `SoundChex` repo (`routes/api.php`, `/api/v1/*`).
- The native iOS app (`SoundChexiOS`) is the reference client — same API, same
  feature shape (profiles, streaming, downloads, playlists, admin, lyrics).
