# Flare Log (Android)

Phone version of the Flare Log desktop app, with two extra questions in the form,
placed below the dates and duration: "Had M?" and "Had S?". Each shows a 1-10
dropdown when answered Yes.

## Get the APK (no Android Studio needed)

1. Create a free account at https://github.com and make a new repository (private is fine).
2. Upload everything in this folder to it. Use "Add file > Upload files" and drag in
   the contents of this folder. Keep the `.github` folder (it may be hidden; if the
   upload skips it, see the note below).
3. Open the repository's **Actions** tab. The "Build APK" workflow starts by itself
   (or press **Run workflow**). It takes about 3-5 minutes.
4. When it shows a green tick, open the run and download **FlareLog-apk** under
   "Artifacts". Unzip it to get `app-debug.apk`.
5. Send the APK to your Poco M2 Pro (Drive, WhatsApp to yourself, USB), open it, and
   allow "Install unknown apps" when MIUI asks.

Note: if the `.github` folder does not upload, create the file
`.github/workflows/build.yml` in the GitHub web editor ("Add file > Create new file",
type the path with the slashes) and paste in the contents of `build.yml`.

## Notes

- Requires Android 10 or newer (the Poco M2 Pro qualifies).
- Data is stored inside the app. Use Backup > Export regularly; files go to Downloads.
- The app screen lives in `app/src/main/assets/index.html`.
