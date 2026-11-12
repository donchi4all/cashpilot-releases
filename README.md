# CashPilot Android Releases

Signed CashPilot Android builds and the update manifest the app reads. **No source code lives here.**

- **Install CashPilot:** download the `.apk` from the [latest release](../../releases/latest) and open it on your Android phone.
- **Updates:** the app checks `releases/latest/download/cashpilot-update.json` and updates itself in-app.

Every update is checked on the phone before install (SHA-256, package name, version, and CashPilot's signing certificate), so a file that isn't signed by CashPilot is refused.

Releases are published with `scripts/prepare-android-update.sh --publish` from the private mobile repo. Do not upload files here by hand.
