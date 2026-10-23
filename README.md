# KeyFlow Piano 🎹

A sleek Android piano studio prototype with a multi-octave touch keyboard, chord progression builder, playback, generated chord/bass/arpeggio instrumental, note capture, local project saving, and JSON import/export.

## Build APK with GitHub Actions
1. Create a new GitHub repository (for example `KeyFlow-Piano`).
2. Upload the contents of this folder to the repository root (not the folder itself).
3. Open **Actions** and enable workflows if GitHub asks.
4. The workflow runs on every push to `main`/`master`, or start **Build KeyFlow APK** with **Run workflow**.
5. Open the completed run, scroll to **Artifacts**, and download `KeyFlow-Piano-APK`. Unzip it to get `app-debug.apk`.

## Build locally
Requires JDK 17 and Gradle 8.9: `gradle assembleDebug`.

## Current limitations
- Audio synthesis and chord playback work offline in the embedded WebView.
- Project import/export uses JSON. Automatic conversion of arbitrary songs/audio into accurate notes, source separation, and full MIDI import/export are not included in this starter version; those require additional audio/MIDI processing.
