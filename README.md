# SakuraLauncher releases

Public distribution repository for SakuraLauncher and Sakura Setup.
The application source is maintained separately in a private repository.

## Downloads

Installers and update packages appear on the [Releases page](https://github.com/alphaisrllycool/Sakura-Releases/releases) after validation. If no release is listed, the first distribution build is still being prepared.

- Windows x64: use **SakuraSetup-x64.exe** for normal installation.
- macOS Intel: use the SakuraLauncher Installer DMG and copy the application to Applications.
- Apple Silicon is not yet physically validated.

Setup downloads a verified launcher package and prepares Minecraft Java and a private Java runtime. Minecraft and Java are obtained from their respective providers, not redistributed in this repository.

## Updates

A new source-code commit does not trigger an application update. Updates are offered only after a versioned release and its signed beta catalog are published. The launcher asks before downloading and applying an update.

`channels/beta.json` is the signed channel catalog. Each immutable
`launcher-vX.Y.Z` tag contains that release's `updater.json`. Package signatures
and SHA256SUMS accompany the downloadable artifacts. Do not replace published
assets; corrections receive a new version.

Update signatures verify package integrity and origin within Sakura's release
system. They are separate from Apple notarization and Windows code-signing.
Initial packages are local-testing beta builds; do not disable operating-system
security protections to install them.

No Microsoft credentials, private signing keys, user data or Minecraft game
files belong in this repository.
