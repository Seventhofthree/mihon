# Nonbiri (のんびり) — TV reader prototype

Nonbiri means taking it easy. A little reading nook for comics and, eventually, novels.

Based on [Mihon](https://github.com/mihonapp/mihon), Apache-2.0. Upstream license and notices remain in this fork.

## What's in version 0.2.0

- A new display name and cozy reading-nook icon and banner.
- Own Android package ID so it can be tested alongside Mihon Shield **without uninstalling the working build or erasing its settings**.
- The existing Mihon comic browsing and continuous-scroll reader, Android TV launcher and remote controls.
- The physical-keyboard search improvement from the earlier Shield branch.

**Not in this build:** LNReader extension support, a novel reader, and unified novel/comic library.
Those require a new plugin runtime and reading interface; they will be developed separately.

## Signing and updates

This experimental build uses the workflow's default debug/test signature, which may differ on subsequent CI runs.
Do not uninstall a working installation or assume updates will overwrite it. Before moving
to ongoing releases, configure a permanent private Android signing key and back up library/source data.

## Installation test

1. Download `nonbiri-android-tv-arm64` from a successful Actions run.
2. Install alongside Mihon Shield.
3. Check Nonbiri launcher tile, onboarding, source setup, comic browsing, reader controls.
4. Report any unexpected layout/focus or crash issues.
