# Changelog

## 1.2.2 — Short in-app release notes

This release changes how update information is displayed, without shortening the full GitHub changelog.

- The Updates page and download confirmation show at most three concise points instead of the complete release text.
- Added a Full changelog action linking to the complete GitHub history. TVs without a browser show the address for opening on another device.
- The update manifest now supports a separate shortNotes field. Full notes remain intact for GitHub and backward compatibility.
- Older releases without shortNotes are displayed using a bounded excerpt of their existing change bullets; no release text is rewritten on GitHub.
- Long lines are safely shortened for TV readability, including Unicode text.

Button mappings, Accessibility permission handling, launcher artwork, APK checksum/signature verification and Android's installation warnings are unchanged. The app still requires explicit installation confirmation and cannot bypass Android Restricted settings.

## 1.2.1 — Accessibility recovery and status

- Fixed stale connected-state reporting when Android unbinds the Accessibility service; pending gestures are cancelled and connection state is cleared.
- Uses Android's public service-status API to show off, connecting, connected or unavailable states accurately.
- Added Settings → Accessibility help, including current service registration and Android 13+ restricted-settings recovery instructions.
- Added a pre-install warning that Android may require Accessibility approval again after an APK update.
- Health checks run only while the app is visible. No automatic permission grants or forced re-enabling.
- Existing mappings, pause preference, Home artwork and signed-update verification are preserved.

On the tested Android 14 TV, the immediate ON → OFF problem was caused by Android's Restricted settings policy, not a mapper crash. An explicitly authorized, RC45-only device permission repair restored the service. The ordinary APK cannot remove this system restriction itself; some firmware requires approval again after an APK update. If the TV hides the standard Allow restricted settings menu, follow the app's trusted-administrator recovery guidance.

## 1.2 — GitHub updates

- Added Settings → Check for updates and a dedicated Updates page.
- Shows release notes, downloads the APK, validates size, SHA-256, package, version and original signing certificate, then opens Android's confirmation installer.
- Public GitHub releases work without login credentials in the TV app.
- No silent installation, mapping uploads or instant push notifications.

## 1.1 — English interface and artwork

- English menus, messages, action labels and accessibility description.
- RockTek RC45 product photograph and refreshed launcher artwork.
- Existing mappings and app signing identity retained.

## 1.0 — Initial release

- Remote-button learning, input monitor and per-button single/double/long-press actions.
- TV-focused dark interface and local mapping backup/restore.
