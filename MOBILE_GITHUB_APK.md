# Mobile-only APK build

This project is configured so GitHub Actions can build the Android APK without a PC.

## On your Android phone

1. Create a GitHub repository.
2. Upload the **contents of this project** to the repository root (not just the ZIP file).
3. Open **Actions** in the repository.
4. Select **Build Android APK**.
5. Tap **Run workflow**.
6. Wait for the green completed run.
7. Open the completed run and scroll to **Artifacts**.
8. Download **My-Daily-Life-Manager-debug-APK**.
9. Extract the downloaded ZIP and install `app-debug.apk`.

The workflow file is already included at:
`.github/workflows/build-apk.yml`

## If GitHub shows the workflow but does not run it

Open the **Actions** tab, select **Build Android APK**, then use **Run workflow** and choose the default branch.
