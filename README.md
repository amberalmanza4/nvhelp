# Communication Assistant for iPhone

This is a native iPhone app wrapper for the supplied communication board. The app contains the board locally, so the board does not need an internet connection after installation.

## Build it free in the cloud

1. Create a free GitHub account, then create a private repository and upload this entire folder.
2. Create a free account at Codemagic and connect that GitHub repository.
3. Select the `build-unsigned-ios-app` workflow from `codemagic.yaml` and start a build.
4. Download `CommunicationAssistant-unsigned.ipa` from the completed build's artifacts.

## Install it on the iPhone without Xcode

1. On the Mac, download Sideloadly from https://sideloadly.io/.
2. Connect the iPhone with a cable, open Sideloadly, and drag `CommunicationAssistant-unsigned.ipa` into it.
3. Enter an Apple Account when Sideloadly asks, then start the install.
4. On the iPhone, go to **Settings → General → VPN & Device Management**, select the Apple Account under **Developer App**, and tap **Trust**.
5. Open **Communication Assistant** from the Home Screen.

With a free Apple Account, Apple requires refreshing the installed app every seven days. In Sideloadly, enable automatic refresh and leave the Mac on the same Wi-Fi network as the iPhone so it can refresh before expiry.

The page code lives in `CommunicationAssistant/index.html`. Edit that file, commit/upload the change, and rerun the Codemagic build to make a new IPA.
