# Dagestan releases

Installers and automatic updates for the Dagestan desktop client. The
source lives in a private repository; only built releases are published
here.

## Install

Open the latest release and download:

- macOS: `Dagestan_x.y.z_universal.dmg`
- Windows: `Dagestan_x.y.z_x64-setup.exe` (or the `.msi`)

Once installed, the app checks this repository for updates at launch and
offers them in its header. Nothing is downloaded without a click.

## Notes

- macOS builds are not yet signed with an Apple Developer certificate. On
  first open, macOS may refuse the app: right-click the app, choose Open,
  and confirm. Or in a terminal: `xattr -dr com.apple.quarantine /Applications/Dagestan.app`.
- Windows builds are not yet signed: SmartScreen warns on the first
  install. Choose "More info", then "Run anyway".
- The `latest.json` and `.sig` files in each release are what the app
  reads to verify and apply updates; they are not meant to be opened.
