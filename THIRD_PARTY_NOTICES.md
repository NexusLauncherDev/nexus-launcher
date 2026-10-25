# Third-party notices

Nexus Launcher and Nexus Setup include third-party software and fonts. Their authors retain all rights. The binary license in this repository applies only to Nexus-owned product material and does not replace or restrict any third-party license.

## Dependency inventories

Complete Windows x64 runtime dependency inventories, with exact versions, declared SPDX license expressions, and links to the accompanying license text, are provided in [license-inventory.csv](license-inventory.csv) for Rust components and [npm-license-inventory.csv](npm-license-inventory.csv) for JavaScript components. The accompanying texts are in [LICENSES/](LICENSES/). Where an upstream package did not include a copy of its standard license, the matching SPDX license text is included.

## Reciprocal-license source availability

The binaries include unmodified MPL-2.0 components. Their corresponding Source Code Form is available from the versioned upstream crate archives: [cssparser 0.37.0](https://crates.io/crates/cssparser/0.37.0), [cssparser-macros 0.7.1](https://crates.io/crates/cssparser-macros/0.7.1), [dtoa-short 0.3.5](https://crates.io/crates/dtoa-short/0.3.5), [option-ext 0.2.0](https://crates.io/crates/option-ext/0.2.0), and [selectors 0.38.0](https://crates.io/crates/selectors/0.38.0). The MPL-2.0 text is included as [LICENSES/MPL-2.0.txt](LICENSES/MPL-2.0.txt).

## Installer and platform components

The Setup executable contains the Microsoft WebView2 Evergreen bootstrapper. It is verified as Microsoft-signed and is run only if WebView2 is missing. Microsoft documents packaging this bootstrapper with an application at <https://learn.microsoft.com/en-us/microsoft-edge/webview2/concepts/distribution>.

NSIS is used to package the installer. Its complete COPYING notice, including the applicable zlib/libpng, bzip2, Common Public License, and LZMA linking exception terms, is included at [LICENSES/NSIS-COPYING.txt](LICENSES/NSIS-COPYING.txt).

## Font, artwork, and game content

The bundled Manrope font is licensed under SIL Open Font License 1.1; its upstream license and attribution are included with the package inventory and license texts. Nexus illustrations were commissioned for this project and are not Minecraft game assets. This installer does not bundle Minecraft, Java, mods, resource packs, shaders, or other game downloads.

Nexus Launcher is an independent community project and is not affiliated with, endorsed by, or sponsored by Mojang or Microsoft. Names and marks for Minecraft remain the property of their respective owners.
