# SS Carrom Pro — Android starter project

This is an Android Studio Kotlin starter project for the requested ad-free carrom game.

## Included in this starter
- Native Android application shell and branded main menu
- Computer difficulty selection (Easy / Medium / Hard)
- Same-phone 2-player and practice entry points
- Initial Canvas board rendering, striker drag/aim, basic motion, wall bounce and coin collision prototype
- Android share chooser entry point
- Bluetooth permissions declared in the manifest

## Not yet complete / must not be treated as production-ready
- Full tournament and casual rule engines (queen cover, due/foul, turn retention, scoring and match-end validation)
- Calibrated realistic physics and complete striker placement/aim controls
- Strong difficulty-specific AI strategy
- Bluetooth discovery, secure pairing, host/join sockets, synchronized authoritative game state, reconnect and disconnect handling
- Packaging, signing and testing of a release APK on physical Android devices

The Bluetooth menu intentionally explains that networking is not implemented yet. The share action currently shares a project description; it does not attach an APK until a signed APK has been built.

## Build
Open this folder in Android Studio (Giraffe or newer), allow Gradle sync, then use Build > Build Bundle(s) / APK(s) > Build APK(s). For release distribution, create and securely retain a signing key in Android Studio. Do not distribute an unsigned debug build as a final release.

Package: `com.sscarrompro.game`
Min Android: API 23 (Android 6.0)
Target SDK: 35
No ad SDKs, analytics SDKs, INTERNET permission, or in-app purchase libraries are included.
