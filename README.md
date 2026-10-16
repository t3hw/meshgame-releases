# Meshgame releases

Android builds of the Meshgame app. The app pairs a phone with a game on
the Meshgame server at **https://game.t3hw.dev** and reports the phone's
position while the game runs.

The current release is a **beta**. Expect changes and bugs.

## Install

1. Open the [latest release](https://github.com/t3hw/meshgame-releases/releases/latest) on the phone.
2. Download the `.apk` file.
3. Open the file. If Android asks, allow your browser or file manager to install unknown apps.
4. Open Meshgame and scan the invite QR code from your game admin.

To update, install the new APK over the old one. The signing key is the
same for every release, so Android keeps the app's data.

## Check the download

Each release lists the SHA-256 of its APK. Compare it with:

    sha256sum meshgame-v0.1.0-beta-release.apk

The signing certificate's SHA-256 digest is:

    dc35e74f6b238dc76986fe96268357d6b59f69021a40354ab01ffa665ab2d237

Check it with `apksigner verify --print-certs <file>.apk`.
