# Slimería XL

This repository contains the web build expected by Capacitor at `www/index.html` and a GitHub Actions workflow to produce a debug Android APK.

## Build a debug APK from GitHub Actions

1. Push changes to `main` or run **Actions → Build APK → Run workflow**.
2. Wait for the workflow to finish.
3. Download artifact **slimeria-xl-apk** from the workflow run.
4. Extract the artifact and use `app-debug.apk`.

## Web asset expectations

The web app is loaded from `www/index.html` and currently uses this asset layout:

- `www/manifest.webmanifest`
- `www/sw.js`
- `www/icon-192.png`
- `www/icon-512.png`
- `www/fonts/PixelifySans.ttf`
- `www/fonts/PressStart2P-Regular.ttf` (optional, app still runs with fallback fonts if missing)

If game source is replaced or removed, add the game HTML back at `www/index.html` before building an APK.
