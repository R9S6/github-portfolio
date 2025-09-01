# AeroGlide Calculator (Android, Kotlin + Compose)

A tiny aerospace tool that computes **glider horizontal range** and **glide angle** from **altitude (m)** and **glide ratio (L/D)**.

## Demo
<img src="docs/caluclator-demo1.png" width="300" alt="AeroGlide screenshot" />

## Features
- Jetpack Compose UI (Material)
- Input validation
- Physics: `range = altitude × (L/D)`, `glideAngle = atan(1/LD) × 180/π`
- Works on Android 7.0+ (minSdk 24)

## Tech
- Kotlin, Compose Material3
- Android Studio
- Gradle Kotlin DSL

## Build & Run
1. Open in Android Studio (Hedgehog or newer).
2. Create/choose a device (API 33–36 OK).
3. Click **Run ▶**.

### CLI (optional)
```bash
./gradlew assembleDebug
adb install -r app/build/outputs/apk/debug/app-debug.apk

app/
 └─ src/
    └─ main/
       ├─ java/com/example/aeroglidefinalized/MainActivity.kt
       ├─ AndroidManifest.xml
       └─ res/...
README.md
.gitignore
settings.gradle.kts
build.gradle.kts
