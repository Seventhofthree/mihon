# Nonbiri (のんびり) — TV reading prototype

Nonbiri means taking it easy. A little reading nook for comics, manga and—later—novels.

An independent fork built on [Mihon](https://github.com/mihonapp/mihon), licensed under Apache-2.0.
The upstream license and attribution remain intact.

## Version 0.3.0 test: TV interaction and branding

This test build includes:

- Full-screen continuous comic reading as in 0.2.0.
- D-pad Down from Popular/Latest/Filter into the first visible comic.
- Visible focus borders on comic covers, list items, source chips and reader buttons.
- Reader settings controls now receive D-pad arrows when opened; initial focus moves to the first toolbar button.
- Settings Search suppresses on-screen keyboards when a physical keyboard is detected.
- Nonbiri cat/book splash, icon, home branding and links to this project.

### Known constraints

- TV keyboard visibility depends on the physical-keyboard hardware configuration; test on real Shield.
- Some other settings text fields may need the same treatment.
- This test app is **Nonbiri Preview** with a *separate* package ID from 0.2.0, so the debug-signed APK can be installed without uninstalling or risking existing 0.2.0 data.
- Preview is not a permanent install/update channel. We still need a stable, private signing key.
- LNReader plugin support, web novels and a unified library are **not yet included**.

## Installation and test steps

1. Download the `nonbiri-preview-0.3.0-arm64` artifact on the matching GitHub Actions run.
2. Extract its APK and sideload **Nonbiri Preview** alongside Nonbiri 0.2.0 and Mihon Shield.
3. In BatCave, focus Popular/Latest/Filter, press **Down** and test selection of the first comic.
4. In a comic, press OK to open the controls. The focus should land on the reading mode icon and left/right should navigate other icons.
5. With the physical keyboard connected, open **Settings → Search settings**; on-screen keyboard should stay hidden and typing/Enter should still work. Check remote-only mode as well.
6. Check launcher icon, startup screen, About links and Getting Started.
7. Report unexpected focus, navigation, or crash behavior.

No new upstream Mihon social links should be presented as Nonbiri's own accounts.
