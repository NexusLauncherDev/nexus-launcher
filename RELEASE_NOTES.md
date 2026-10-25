# Nexus Launcher 2.1.0-beta.1

The first public beta brings together instance management, Modrinth browsing, Nexus Studio, Cinematic Launch, Mod Intelligence, Crash Investigator, Nexus Companion, and the redesigned Nexus Setup 2.0 installer.

## Download and install

- Download `NexusSetup.exe` and `SHA256SUMS.txt` from the assets attached to this release.
- Compare the downloaded installer's SHA-256 with the checksum file before running it.
- Setup installs for the current Windows user, lets you choose the destination folder, and can update an existing installation.
- The installer is not Authenticode-signed. Windows SmartScreen may show an unknown-publisher warning.
- If WebView2 is missing, Setup offers Microsoft's signed Evergreen bootstrapper.

## Beta limitations

- Tested on one Windows 11 24H2 x64 machine (build 26100). Other Windows versions, Windows Server, and ARM devices have not been verified.
- Microsoft sign-in and CurseForge downloads are unavailable in this beta.
- Automatic launcher updates are not available. Download a later installer from GitHub Releases and run it manually.
- Network services, account flows, loaders, and game versions have not been tested in every combination.
- Nexus Launcher is an independent project and is not affiliated with Mojang or Microsoft.

See [README.md](README.md) for the full feature list, install guidance, and feedback details. See [README.ru.md](README.ru.md) for Russian.

## Verification

Checks run on 2026-10-25:

- 98 Rust tests passed; 11 live or opt-in tests were intentionally ignored.
- The full browser UI run passed 80 of 82 cases. The two affected checks passed when rerun separately after updating the version-specific Classic screenshot references (Classic 2/2; music panel 3/3).
- Native Setup checks passed for both languages, seven scenes, supported window sizes, invalid-folder recovery, installation, launch, and uninstall on the test host.
- `npm audit --omit=dev` reported no known vulnerabilities for either JavaScript lockfile. `cargo audit` reported no vulnerable advisories in either Rust lockfile. Its remaining maintenance and soundness warnings concern crates that are not part of the Windows x64 dependency graph.


