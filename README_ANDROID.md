# ZERO POINT — GitHub Android build

This archive contains the original Bevy 0.15.3 game source plus a GitHub Actions workflow.

## Build from GitHub on a phone

1. Upload the **contents** of this archive to the root of your `ZERO-POINT` GitHub repository.
2. Open the repository's **Actions** tab.
3. If GitHub asks, enable Actions for the repository.
4. Open **Build ZERO POINT Android APK** and tap **Run workflow**. A push to `main` also starts a build automatically.
5. Wait for the run to finish. Under **Artifacts**, download `ZERO-POINT-APK`.
6. Extract the downloaded artifact ZIP; it contains the APK.

## Notes

- The workflow builds an Android APK for 64-bit ARM devices (`arm64-v8a`).
- It downloads the Android Gradle project template from the matching Bevy `v0.15.3` tag at build time.
- This is a build setup, not a verified APK. The first GitHub run is the actual compile test; if it fails, share the failed log and the setup can be corrected.
- The game is an early prototype. Touch controls and performance still need testing on a real phone.
