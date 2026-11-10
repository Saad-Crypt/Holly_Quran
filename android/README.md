# Holly Quran for Android

This Android wrapper packages the existing `Holly_Quran/index.html` as a native-installable APK using Android WebView.

## Features
- Preserves the original Arabic Quran web interface.
- Uses a stable HTTPS app asset origin so browser storage such as IndexedDB and localStorage can persist.
- Retains internet access for Quran text APIs, recitation audio, and web fonts.
- Cached content and saved settings may remain available offline, depending on what the web app has already downloaded.

## Build locally
Requirements: JDK 17, Android SDK 35, and Gradle 8.10.2.

From this directory:
```bash
gradle assembleDebug
```

APK output:
`app/build/outputs/apk/debug/app-debug.apk`

## Build on GitHub
Open the repository's Actions tab and run **Build Holly Quran APK**, or push a change under `android/`. Download the generated `Holly-Quran-debug-apk` artifact from the successful workflow run.

The debug APK is suitable for testing and sideloading. A signed release APK should be created separately before public distribution.
