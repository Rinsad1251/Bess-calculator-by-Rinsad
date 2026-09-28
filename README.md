# Rinsad's BESS Sizing Calculator – Android app

Offline Android app that runs the BESS sizing calculator. The calculator lives in `app/src/main/assets/index.html`.

## Get the APK with GitHub (no install needed)
1. Create a free account at github.com and make a new repository (e.g. `bess-calculator`).
2. Click **Add file → Upload files**, drag in everything from this folder (including the `.github` folder), and commit.
3. Open the **Actions** tab. The "Build APK" job runs automatically (about 3–5 minutes).
4. When it shows a green tick, open the run and download **BESS-Calculator-APK** under Artifacts. Unzip it to get `app-debug.apk`.
5. Copy the APK to your phone and tap it. Allow "Install unknown apps" for your file manager when Android asks.

Tip: on some computers the upload page hides folders starting with a dot. If `.github` is missing, create the file
`.github/workflows/build-apk.yml` in GitHub with **Add file → Create new file** and paste its contents.

## Build with Android Studio
Open this folder in Android Studio (Hedgehog or newer), let Gradle sync, then **Build → Build APK(s)**.

## Updating the calculator
Replace `app/src/main/assets/index.html`, raise `versionCode` in `app/build.gradle`, and rebuild.
