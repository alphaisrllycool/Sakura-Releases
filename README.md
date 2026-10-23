# SakuraLauncher releases

Public distribution repository for SakuraLauncher and Sakura Setup. The application source is maintained separately in a private repository.

## Sakura 0.2.4 beta

The public beta is available now.

- [Launcher updates and recovery packages](https://github.com/alphaisrllycool/Sakura-Releases/releases/tag/launcher-v0.2.4)
- [Guided installer: Windows setup and macOS setup DMG](https://github.com/alphaisrllycool/Sakura-Releases/releases/tag/setup-v0.2.4)
- [All releases](https://github.com/alphaisrllycool/Sakura-Releases/releases)

**macOS correction:** The installer DMG is now **SakuraLauncher-Installer_0.2.4_macos-x64.dmg**. The earlier **SakuraLauncher_0.2.4_x64.dmg** contains the launcher app directly, not the setup wizard. Use the newly named installer DMG for guided setup. Its SHA-256 and build manifest are attached to the setup release.

**Windows repair:** Do not use the previously attached **SakuraSetup_0.2.4_windows-x64-repair.zip**; it is defective. For Windows launcher repair, use **SakuraLauncher_0.2.4_x64-setup.exe** from the launcher release. **SakuraSetup-x64.exe** remains the normal setup bootstrapper.

Windows x64 and macOS Intel are provided; Apple Silicon is not included. Windows was cross-compiled on macOS, and native Windows installation, repair, and update acceptance remain pending. Native end-to-end installation of the corrected macOS wizard on a clean account also remains pending. Microsoft account access to Minecraft Services awaits separate authorization and a real-account test.

The macOS app is not Apple Developer ID signed or notarized; the Windows setup is not Authenticode-signed. Antivirus review is unresolved, and Sakura has not verified the detections as false positives. Do not disable Gatekeeper, Defender, or other security protections.

If an existing installation cannot update because an interrupted session blocks its old updater, use the platform-specific recovery instructions and files in the launcher release. Preserve Minecraft worlds, profiles, mods, and account data. Do not uninstall with data removal.

## Downloads

- **Windows x64 normal setup:** **SakuraSetup-x64.exe** from the setup release.
- **macOS Intel guided setup:** **SakuraLauncher-Installer_0.2.4_macos-x64.dmg** from the setup release.
- **Windows launcher repair:** **SakuraLauncher_0.2.4_x64-setup.exe** from the launcher release.
- **macOS launcher repair:** **SakuraLauncher_0.2.4_macos-x64-repair.zip** from the launcher release.

The setup downloads verified launcher components and prepares Minecraft Java and a private Java runtime. Minecraft and Java are obtained from their respective providers; this repository does not redistribute them. Check the applicable release's SHA256SUMS files and signature files when verifying downloads.

## Updates

The launcher checks the signed beta catalog and asks before downloading and applying an update. An unavailable feed does not block use of the installed launcher. The current signed beta channel is [channels/beta.json](https://raw.githubusercontent.com/alphaisrllycool/Sakura-Releases/main/channels/beta.json). The immutable launcher-vX.Y.Z tag contains that version's updater.json.

Sakura updater/catalog signatures verify package integrity and origin within Sakura's release system. They are separate from Apple notarization and Windows code-signing. Do not replace published assets; corrections receive a new version. No Microsoft credentials, private signing keys, user data, or Minecraft game files belong in this repository.

Sakura 0.2.4 is a beta. Review release notes and limitations before installing.
