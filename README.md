# Estimation Scorekeeper for Android

Score keeper for the Estimation card game: single players or 2 v 2 teams, online (Jawaker) or classic rules. Everything works offline, and games are saved on the phone.

## Download

**[Download Estimation.apk](https://github.com/Qodsy95/estimation-app/releases/latest/download/Estimation.apk)**

1. Open the link above on your Android phone and download the file.
2. Open the downloaded **Estimation.apk**. The first time, Android asks you to allow installs from your browser or Files app. Allow it, then tap **Install**.
3. The app shows up as **Estimation** with the cards icon.

New versions install over the old one and keep your saved games.

## How it's built

The app is a web page (`app/src/main/assets/www/index.html`) shown full screen in an Android WebView. Every push to `main` runs the **Build APK** workflow in GitHub Actions, which builds the APK and publishes it as the latest release.

The signing key in `signing/` is in the repo on purpose, so every build is signed the same way and updates install over each other. It's fine for installing on your own phones. Don't use it for the Play Store.
