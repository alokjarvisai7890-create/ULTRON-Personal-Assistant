# ULTRON — Your Personal AI

An Android 10+ starter project for a Hindi/English personal assistant with a blue-neon futuristic interface.

## What this ZIP contains
- Kotlin + Jetpack Compose Android project
- Voice-input prototype using Android speech recognition
- GitHub Actions workflow to build a debug APK
- Basic project documentation

## Important status
This is a **starter prototype**, not the complete assistant described in the planning conversation. AI services, persistent memory, wake-word detection, WhatsApp/Telegram integrations, phone automation, smart-home integrations, navigation, music controls, PIN/biometric lock, and notification reading are not implemented yet. These require separate integrations, user permissions, provider APIs, and device-specific testing.

Android and Xiaomi/Redmi background restrictions mean always-on microphone listening and automatic boot behavior cannot be guaranteed. Do not use Accessibility to bypass Android security or app restrictions. Sensitive actions should always require user confirmation.

## Build with GitHub Actions (phone-friendly)
1. Create a public GitHub repository named `ULTRON-Personal-Assistant`.
2. Upload the **contents** of this ZIP to the repository root (not the enclosing folder).
3. Open the repository's **Actions** tab.
4. Enable Actions if GitHub asks.
5. Run **Android APK** using **Run workflow**, or push a commit to `main`.
6. Open the completed workflow run and download the `ULTRON-debug-apk` artifact.
7. Extract the artifact ZIP on Android and install `app-debug.apk`. You may need to allow installs from your browser/file manager.

## Local build
Requires JDK 17 and Gradle 8.9+:
```bash
gradle assembleDebug
```

## Package details
- Application ID: `com.ultron.personalassistant`
- Minimum Android: 10 (API 29)
- Compile/target SDK: 35
- Version: `0.1.0`

## Privacy and security
- Never put passwords, OTPs, API keys, or signing keys in source code.
- Use official OAuth/provider sign-in for connected services.
- Request permissions only when a feature is used.
- This starter app currently requests microphone permission only when voice input is tapped.
- Public repositories are visible to everyone. Do not upload personal data or secrets.
