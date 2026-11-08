# Mihon Shield MVP 0.1

Experimental NVIDIA Shield / Android TV build of Mihon. Based on
[mihonapp/mihon](https://github.com/mihonapp/mihon) (Apache License 2.0).

Changes:
- Independent app ID and display name so original Mihon may coexist.
- Android TV launcher intent, touch-optional device declarations, and TV banner.
- Dedicated book icon for the fork.
- Remote OK / keyboard Enter toggles reader controls when hidden.
- Existing arrow / PageUp / PageDown reading shortcuts remain in place.
- Disable official Mihon update checker on custom builds.
- ARM64 APK build on each push to the shield/mvp-0.1 branch.

**Not tested on a physical Shield or compiled before this commit.**
Menus, onboarding storage picker, extension APK installation, focus behavior,
and network reading need real-device validation.

## Test plan
1. Download APK from Actions build artifact and sideload it on Shield.
2. Verify launcher tile, onboarding, and storage directory picker.
3. Use mouse/keyboard to browse and install a trusted compatible source.
4. Open online comic pages without downloading an entire issue.
5. Test arrows and OK/Back on remote; confirm reading progress.
6. Check cache footprint and whether clearing cache leaves progress intact.

This branch is intentionally separate from fork main until the initial
device tests are complete. The CI build is debug/test signed, not a
production-stable update key.
