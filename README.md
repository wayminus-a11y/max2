# MAX – Android Offline App (Starter Source)

This repository is a **starter Android Studio/Kotlin project**, not a completed clone of the uploaded Panda APK.

## Included
- Kotlin Android application named MAX
- Android manifest with no `INTERNET` permission
- Android backup disabled by default
- Cleartext traffic disabled
- Android Keystore AES-GCM helper (`SecureLocalStore.kt`)
- Marathi setup and security notes

## Not yet implemented
- Panda app's complete screens and feature set
- Local AI model, inference engine, and model assets
- Offline speech recognition / text-to-speech and wake-word pipeline
- Browser automation
- Accessibility automation
- Data screens, persistent database integration, import/export, backup/restore
- Automated tests and a signed release APK

The uploaded APK is a compiled application package. Its original complete source code cannot be recovered reliably from the APK alone. This project is an independent starting implementation; it does not contain the original app's private source, server code, or proprietary assets.

## Open in Android Studio
1. Extract this ZIP.
2. Open the `MAX_Android_Project` folder in Android Studio.
3. Allow Gradle sync and install the required Android SDK components.
4. Build using **Build → Build APK(s)**.

A compatible Android SDK/Gradle build environment is required. This ZIP has not been compiled into a verified APK in this workspace.

## Offline and security notes
- The manifest currently does not request internet access. Review all future dependencies and manifest merges before release.
- The encryption helper is not yet connected to an app database or user data flow.
- Keep signing keys outside GitHub. Never commit passwords, tokens, private keys, or user data.
- Do not claim the app is fully secure until permissions, dependencies, storage, backup/restore, and runtime network behavior have been tested.
