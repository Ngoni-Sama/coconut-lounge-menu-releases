# Coconut Lounge Menu — releases

Published builds of the Coconut Lounge kiosk menu app for the restaurant's Android tablets.

- **Menu app:** each [release](../../releases) has the APK attached (`CoconutLoungeMenu-vX.Y.Z.apk`).
- **Tablet updater:** `Coconut Tablet Updater.exe` (Windows) downloads the newest release automatically
  and updates the tablets plugged into the PC over USB. Updating keeps each tablet's activation,
  menu edits, orders and admin PIN.

- **Kiosk app:** `kiosk/` holds the FreeKiosk APK the updater installs on new tablets
  (`kiosk.json` lists the file, version and SHA-256 checksum). FreeKiosk is
  [open source](https://github.com/RushB-fr/freekiosk) under the MIT licence, see `kiosk/FREEKIOSK-LICENSE.txt`.
  To change the FreeKiosk version, replace the APK and update `kiosk.json` (file, version, size, sha256).

New version: create a release tagged like `v1.3.4` with the APK attached. Updaters pick it up the
next time they start, or when someone clicks "Check for a new version".
