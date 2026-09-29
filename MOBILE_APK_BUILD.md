# My Daily Life Manager — Android APK build

This is the AI Studio React/Vite project prepared for Android packaging with Capacitor.

## Requirements
- Node.js 20+ (Node 22 recommended)
- Android Studio
- Android SDK + an installed Android platform/build tools
- JDK 17+ (JDK 21 is also suitable for the current Android toolchain)

## First-time setup

```bash
npm install
npx cap add android
```

If Capacitor asks to install a package, accept it.

## Build debug APK

```bash
npm run apk:debug
```

The APK will normally be at:

`android/app/build/outputs/apk/debug/app-debug.apk`

## Open in Android Studio

```bash
npm run android
```

Then choose **Build > Build APK(s)** in Android Studio.

## Release APK

For a Play Store/release APK, create your own signing key and use Android Studio's **Generate Signed Bundle / APK** wizard. Do not put a production keystore or passwords into this project ZIP.

## Gemini API key

The original AI Studio app expects `GEMINI_API_KEY` through the web app environment. Do not hard-code a private API key into a public APK. For production, put Gemini calls behind a secure server/API proxy or use an appropriate authenticated backend.
