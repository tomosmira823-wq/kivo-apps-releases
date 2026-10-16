# Kivo apps — releases

Windows installers for the Kivo apps from Kivo Studio (https://kivostudio.uk). The apps check `latest.json` here on start-up and offer to update when a newer version is listed.

| App | Version | Installer |
|---|---|---|
| KivoPDF | 0.8.0 | [Download](https://raw.githubusercontent.com/tomosmira823-wq/kivo-apps-releases/main/KivoPDF/KivoPDF-0.8.0-windows-x64-setup.exe) |
| KivoWrite | 0.7.0 | [Download](https://raw.githubusercontent.com/tomosmira823-wq/kivo-apps-releases/main/KivoWrite/KivoWrite-0.7.0-windows-x64-setup.exe) |

## Releasing an update

1. Bump the version and build the installer.
2. Put it in the app's folder here and update its `version`, `url` and `sha256` in `latest.json` (the apps refuse a download whose SHA-256 doesn't match).
3. Commit and push. Apps pick it up next time they open.
