# GradeFlow (Android)

Offline WebView wrapper around the E-Grade Book HTML (app/src/main/assets/index.html).

## Build the APK
1. Open this folder in Android Studio (Ladybug or newer) and let Gradle sync.
2. Build > Build Bundle(s) / APK(s) > Build APK(s)
3. Output: app/build/outputs/apk/debug/GradeFlow-debug.apk  (copy it to the phone and install)

No Android Studio? Push this folder to a GitHub repo; the workflow in .github/workflows
builds the APK (Actions > Build GradeFlow APK > Artifacts).

## Notes
- Exports/backups are saved in Downloads/GradeFlow.
- The app has no INTERNET permission (fully offline).
- Data from the HTML opened in a browser is NOT shared with the app: make a JSON backup in the
  browser version and restore it inside the app (Settings > restore).
- To update the gradebook later, replace app/src/main/assets/index.html and rebuild.
