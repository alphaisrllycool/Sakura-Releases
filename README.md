# SakuraLauncher releases

Public distribution repository for SakuraLauncher and Sakura Setup. Application source is maintained separately.

## Sakura 0.2.5 beta

- [Launcher, in-app updates and recovery files](https://github.com/alphaisrllycool/Sakura-Releases/releases/tag/launcher-v0.2.5)
- [Installers for Windows and macOS](https://github.com/alphaisrllycool/Sakura-Releases/releases/tag/setup-v0.2.5)
- [All releases](https://github.com/alphaisrllycool/Sakura-Releases/releases)

### Downloads

- **Windows x64 installer / repair:** `SakuraSetup-x64.exe` from the setup release.
- **Windows launcher updater:** `SakuraLauncher_0.2.5_x64-setup.exe` from the launcher release.
- **macOS Intel guided installer:** `SakuraLauncher-Installer_0.2.5_macos-x64.dmg` from the setup release.
- **macOS Intel launcher app:** `SakuraLauncher_0.2.5_macos-x64.dmg` from the setup release.
- **macOS Intel manual recovery:** `SakuraLauncher_0.2.5_macos-x64-repair.zip` from either release.

Sakura 0.2.5 addresses stale session reservations that could block launching Minecraft or installing versions after an interrupted session. If an older launcher cannot update, run the installer for your platform over the existing installation. Preserve player data, profiles, mods, accounts, and worlds; do not uninstall with data removal. See `RECOVERY.md` attached to the launcher release.

The owner confirmed Windows download, installation, and Minecraft gameplay. macOS package signatures and DMGs were verified, but native installation acceptance remains pending. This release provides Windows x64 and macOS Intel; Apple Silicon is not included. The Windows setup has no Authenticode signature. The macOS app and installer are not Developer ID signed or notarized; do not disable Gatekeeper, Defender, or other security protections. Tauri updater packages and the signed beta catalog have been verified. Antivirus detections have not been confirmed as false positives.

Microsoft OAuth sign-in does not itself grant Minecraft Services access. That separate approval remains pending, so do not treat this beta as confirmation that Microsoft Minecraft authentication works for every account.

## Updates

The launcher checks the signed beta catalog and asks before downloading and applying an update. An unavailable feed does not block use of the installed launcher. The current signed beta channel is [channels/beta.json](https://raw.githubusercontent.com/alphaisrllycool/Sakura-Releases/main/channels/beta.json). The immutable `launcher-vX.Y.Z` tag contains that version's `updater.json`.

Sakura updater/catalog signatures verify package integrity and origin within Sakura's release system. They are separate from Apple notarization and Windows code signing. Corrections receive a new version; published assets are not replaced. No Microsoft credentials, private signing keys, user data, or Minecraft game files belong in this repository.
