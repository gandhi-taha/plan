# Improvement Plan

A personal planner and tracker for study, thesis, gym and French. It runs entirely in the browser,
works offline, and installs on Android as an app. Progress syncs through your own Google Drive.

## Files
- `index.html`: the whole app
- `manifest.webmanifest`, `sw.js`, `icon-*.png`: let Android install it and run it offline

## Use on a computer
Open `index.html` in Chrome, Edge or Firefox. Data is saved in that browser.

## Install on Android
1. Create a public GitHub repository named `plan` and upload these files.
2. In the repository: Settings > Pages > Deploy from branch > `main` / root.
3. On your phone, open `https://gandhi-taha.github.io/plan/` in Chrome, then menu > Add to Home screen.

The repository holds only the app code. Your progress is never in it.

## Google Drive sync
- **No setup:** Plan & settings > "Save backup to Drive" (Android share menu > Drive) and "Load backup from Drive".
- **Automatic:** create a free Google OAuth client ID (steps are in the app under Plan & settings > Google Drive),
  with your GitHub Pages address as an authorised JavaScript origin. Paste it in the app and tap Connect & sync on each device.
  The app only gets access to its own hidden app-data folder in your Drive.
