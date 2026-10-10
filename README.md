# Zexi Bot Android wrapper

This Android app opens **https://zexibot.netlify.app/** in a mobile WebView.
It supports JavaScript, browser storage, Android back navigation, and file selection for upload fields.

## Build APK using GitHub Actions
1. Upload this project to a new GitHub repository (or replace files in a dedicated Android-app repository).
2. Open **Actions** and run **Build Zexi Bot APK** (or push to `main`).
3. Open the completed workflow run and download the `ZexiBot-debug-APK` artifact.
4. Extract the artifact ZIP and install `app-debug.apk` on your Android device.

This workflow produces a **debug APK** for testing/installation. A Play Store release requires a separately signed release build and a secure signing key.

## App icon
The supplied base64 image string in the request appeared truncated, so this project uses a temporary vector icon. Replace `app/src/main/res/drawable/ic_launcher.xml` with the final brand artwork when you have the complete image file.

## Notes
- This is a WebView wrapper, not an offline native rewrite. The website and its backend must remain online.
- The app does not contain Telegram bot tokens or backend secrets.
