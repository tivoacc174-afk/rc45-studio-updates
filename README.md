# RC45 Studio updates

Public APK releases and release notes for RC45 Studio, an Android TV remote-button mapper.
This repository does not contain signing keys, GitHub credentials or users' button mappings.

## Download and update

Download the APK from the [latest published release](../../releases/latest).
Versions with the in-app updater can use **Settings → Check for updates** or the **Updates** page.
Read the release notes, choose **Download & install**, and confirm installation in Android.
If Android requests it, allow RC45 Studio under **Install unknown apps**, return to the app,
and choose **Install update** again.

Publishing a release makes it available to the app's next manual check. It does not silently
install an APK or send an instant push notification.

## Integrity and privacy

Each release includes the APK, `update.json` and `SHA256SUMS.txt`.
The app checks the APK size, SHA-256, package name, version and original signing certificate.
Existing mappings are preserved by an in-place update. Never uninstall or clear app data to update.

Updates use public HTTPS GitHub downloads without an account or token in the TV app.
Button events, mappings and screen content are not uploaded. GitHub receives normal network
requests when the user checks for or downloads an update.

The app requires Android 8.0/API 26 or later. Some IR power, microphone and OEM shortcut buttons
may be handled directly by the device firmware rather than Android key filtering.

RockTek RC45 product imagery referenced by the app: [TV4U product page](https://tv4u.com.ua/ru/product/rocktek-rc45/).
RockTek is a product brand; this personal app is not an official RockTek firmware update service.
