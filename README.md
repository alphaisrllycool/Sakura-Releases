# SakuraLauncher releases

Public distribution repository for SakuraLauncher and Sakura Setup. The application source is maintained separately in a private repository.

## Sakura 0.2.4 beta

The public beta is available now.

- [Launcher update packages and recovery downloads](https://github.com/alphaisrllycool/Sakura-Releases/releases/tag/launcher-v0.2.4)
- [Windows setup and macOS installer DMG](https://github.com/alphaisrllycool/Sakura-Releases/releases/tag/setup-v0.2.4)
- [All releases](https://github.com/alphaisrllycool/Sakura-Releases/releases)

Windows x64 and macOS Intel are provided. Apple Silicon is not included. The Windows build was cross-compiled on macOS; native Windows install, repair, and update acceptance is still pending. Microsoft account access to Minecraft Services is also pending its separate authorization and real-account test.

The macOS DMG is not signed with an Apple Developer ID or notarized, and the Windows setup is not Authenticode-signed. Some antivirus vendors have flagged the setup; that review is unresolved. Sakura has not verified those detections as false positives. Do not disable Gatekeeper, Defender, or other security protections to install it.

If an existing installation cannot update because an interrupted session blocks its old updater, use the platform-specific recovery instructions and files in the launcher release. Preserve your Minecraft worlds, profiles, mods, and account data. Do not uninstall with data removal.

## Downloads

- **Windows x64:** use `SakuraSetup-x64.exe` for normal setup. The launcher release also includes the signed updater package and recovery files.
- **macOS Intel:** use `SakuraLauncher_0.2.4_macos-x64.dmg`. The launcher release includes the signed updater package and a manual recovery archive.

Setup downloads verified launcher components and prepares Minecraft Java and a private Java runtime. Minecraft and Java are obtained from their respective providers; this repository does not redistribute them. Check each release's `SHA256SUMS.txt` and signature files when verifying downloads.

## Updates

The launcher checks the signed beta catalog and asks before downloading and applying an update. An unavailable feed does not block use of the installed launcher. The current signed beta channel is [`channels/beta.json`](https://raw.githubusercontent.com/alphaisrllycool/Sakura-Releases/main/channels/beta.json). The immutable `launcher-vX.Y.Z` tag contains that version's `updater.json`.

Sakura updater/catalog signatures verify package integrity and origin within Sakura's release system. They are separate from Apple notarization and Windows code-signing. Do not replace published assets; corrections receive a new version. No Microsoft credentials, private signing keys, user data, or Minecraft game files belong in this repository.

Sakura 0.2.4 is a beta. Review the release notes and limitations before installing.
