<div align="center">
  <img src="assets/banner.png" alt="Nexus Setup welcome screen" width="100%">
  <h1>Nexus Launcher</h1>
  <p>A Windows launcher for managing and playing Minecraft Java Edition instances.</p>
  <p><a href="https://github.com/NexusLauncherDev/nexus-launcher/releases/download/v2.1.0-beta.1/NexusSetup.exe"><strong>Download Nexus Launcher 2.1.0 Beta 1</strong></a></p>
  <p><strong>Open beta · Windows x64 · Unsigned installer</strong></p>
  <p><a href="README.ru.md">Русская версия</a> · <a href="https://github.com/NexusLauncherDev/nexus-launcher/releases/tag/v2.1.0-beta.1">Release notes</a> · <a href="https://github.com/NexusLauncherDev/nexus-launcher/issues/new/choose">Report a bug or request a feature</a></p>
</div>

Nexus brings instance management, Modrinth content, launch diagnostics, and a customizable workspace together in one desktop app. This is an early beta; some integrations and operating-system combinations have not been verified.

## What is in the beta

- **Instance management:** create and organize isolated game instances, review their content, and launch them.
- **Modrinth catalog:** browse projects and install compatible content into an instance.
- **Nexus Studio:** use the alternate workspace for library organization and instance controls.
- **Cinematic Launch:** a launch surface with live progress and reduced-motion support.
- **Mod Intelligence:** scan local mod files and review evidence-backed compatibility findings.
- **Crash Investigator:** inspect local game logs and review a bounded, redacted diagnostic summary.
- **Nexus Companion:** view measured activity for a tracked game process.
- **Nexus Setup 2.0:** choose an installation folder, install or update the launcher, and verify installed files.

Feature availability depends on the selected account, game files, network services, and instance configuration. See [known limitations](#known-limitations) before installing.

## Screenshots

The banner above shows the real Nexus Setup welcome screen. The [Setup showcase](assets/screenshots/setup-showcase.png) is another capture from the shipped installer, using original project artwork.

## System requirements

- Windows x64. The current beta has been exercised on one Windows 11 24H2 x64 machine (build 26100). This is a test result, not a claim that other Windows editions are supported.
- An internet connection for game files, Modrinth content, and the WebView2 prerequisite when it is missing.
- Minecraft Java Edition files and any account or game entitlement required by the selected profile.

Windows 10, Windows Server, ARM devices, and other Windows builds were not verified for this release.

## Install

1. Download `NexusSetup.exe` from the [v2.1.0-beta.1 release](https://github.com/NexusLauncherDev/nexus-launcher/releases/tag/v2.1.0-beta.1).
2. Optionally compare its SHA-256 with `SHA256SUMS.txt` attached to that release.
3. Run the installer and choose the destination folder. Setup installs for the current Windows user; it does not require you to replace an existing installation path.
4. Launch Nexus from the completion screen or Start menu.

The installer is not Authenticode-signed. Windows SmartScreen may show an unknown-publisher warning. Verify the downloaded file and its SHA-256 before deciding whether to run it. If WebView2 is missing, Setup offers Microsoft's signed Evergreen bootstrapper; that step needs an internet connection.

Setup has been tested in an isolated install and update flow. The release notes list the test scope and anything that could not be checked on this machine. Do not interrupt Setup after its file-commit stage begins.

## Updating

The launcher does not currently have a verified automatic update mechanism. Download the next installer from GitHub Releases and run it over the existing installation. Setup detects the existing folder and preserves launcher data it does not manage.

## Known limitations

- This beta was tested on a single Windows 11 24H2 x64 host; compatibility with other Windows versions is unverified.
- The installer is unsigned, so SmartScreen can identify it as an unknown publisher.
- Microsoft sign-in and CurseForge downloads are not enabled in this beta. Provider availability can change as integrations are completed.
- Automatic launcher updates are not available; update manually from Releases.
- Online services, authentication, mod loaders, and Minecraft versions have not all been tested in every combination.
- Nexus Launcher is an independent community project. It is not affiliated with, endorsed by, or sponsored by Mojang or Microsoft.

## Feedback

Use [Issues](https://github.com/NexusLauncherDev/nexus-launcher/issues/new/choose) for reproducible bug reports and feature requests. Before attaching logs, remove account names, access tokens, email addresses, and private file paths. Do not post credentials or authentication tokens.

## License

Nexus Launcher and Nexus Setup are proprietary binary products. The source code is not included in this repository. The [binary license](LICENSE) covers the Nexus-owned parts only; third-party components remain under their respective terms in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
