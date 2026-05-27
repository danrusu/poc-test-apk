# poc-test-apk

A minimal Android login application.

## Features

- Login screen with username and password fields
- Valid credentials: `tester` / `passw0rd`
- On successful login: navigates to a welcome screen displaying **"Hello tester!"**
- On invalid login: shows an error message

## Requirements

- Android Studio (Hedgehog or newer) **or** JDK 17+ with the Android SDK installed
- Android SDK with `compileSdk 34` and `minSdk 21`

## Build

### Using Android Studio
1. Open the repository root folder in Android Studio.
2. Let Gradle sync complete.
3. Click **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
4. The debug APK will be at `app/build/outputs/apk/debug/app-debug.apk`.

### Using the command line

```bash
# On macOS/Linux
./gradlew assembleDebug

# On Windows
gradlew.bat assembleDebug
```

The APK will be generated at `app/build/outputs/apk/debug/app-debug.apk`.

## Run

Install on a connected device or emulator:

```bash
./gradlew installDebug
```