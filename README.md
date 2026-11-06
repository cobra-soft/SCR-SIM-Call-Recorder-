# SIM Call Recorder — MVP scaffold

Android (Kotlin + Jetpack Compose) project scaffold. Not buildable on-device; open in Android Studio on a PC.

## Prerequisites
- JDK 17
- Android Studio (latest stable) with SDK 35
- Gradle 8.10 (wrapper included)

## Build debug APK
```
./gradlew assembleDebug
```

## Next steps (phases)
1. Dialer: keypad, SIM selector, place call (TelecomManager/SubscriptionManager).
2. Recording: ForegroundCallService, RecordingEngine VOICE_CALL + fallback, status.
3. Legal: LegalPolicyEngine region/consent, onboarding gates.
4. UI polish: Monet, animations, localization.

## Notes
- minSdk 31 (Monet). Full call recording may be unavailable on modern Android; app must report honest status.
- Recording/telephony logic is stubbed with TODOs referencing TZ sections.
