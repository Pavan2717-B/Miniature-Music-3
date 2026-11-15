# Miniature – Android app (WebView wrapper)

Page: app/src/main/html/index.html (songs are in app/src/main/songs/ and are merged back in at build time).
Logo: already converted into all launcher icons.

## Build the APK with GitHub (no installs)
1. Upload everything in this folder to your repo (the .github folder must be included).
2. Actions tab -> "Build APK" -> Run workflow.
3. Download "Miniature-APK" from the finished run, unzip, install app-debug.apk.

## Updating later
1. Open tools/strip-songs.html in your browser, pick your new full HTML, download the small index.html it gives you.
2. Upload it to app/src/main/html/index.html on GitHub (replace). Songs only if they changed.
3. Raise versionCode in app/build.gradle, commit. The APK builds automatically.
