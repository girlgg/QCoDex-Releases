# QCoDex

[简体中文](README.zh-CN.md)

QCoDex is a Windows x64 workbench for browsing, previewing and exporting supported game assets. This repository provides binary releases and usage information.

## Upcoming preview

0.5.1 is being prepared and is not yet published. [Draft release notes](release-notes/0.5.1.en.md). The download below remains 0.5.0.

## Download

**[Download QCoDex v0.5.0 for Windows x64](https://github.com/girlgg/QCoDex-Releases/releases/download/v0.5.0/QCoDex-0.5.0-windows-x64.zip)** · [Release notes](https://github.com/girlgg/QCoDex-Releases/releases/tag/v0.5.0)

Version 0.5.0 is the first public preview. Download the program ZIP, not GitHub's automatically generated **Source code** archives.

## Requirements and first run

- Windows 11 x64 and a GPU/driver supporting Vulkan 1.3 and the required device features.
- Extract the **entire** ZIP to a folder writable by your account, then run `QCoDex.exe`.
- Qt, the VC++ runtime and application dependencies are bundled. No separate Qt, VC++ Redistributable or development SDK installation is required.
- Select your own game installation when you want to browse assets. The workbench can open without a registered game; game assets are not included.

The program provides asset browsing and search, image/model/material previews, model exports to CAST/FBX/glTF, image exports to PNG/DDS, and supported audio exports to WAV/FLAC. Available operations depend on the actual source format, asset type and required data. English and Simplified Chinese interfaces, light/dark themes and CLI commands are included. Run `QCoDex.exe --help` for CLI usage.

## Data and upgrades

For the upcoming 0.5.1 preview, configuration lives in `config/` beside the executables; the database, caches and user documents default to `data/`. Back up the complete old application folder and extract the new version into a new writable folder. Old settings, registrations, dictionaries and catalogs are not migrated. Do not copy the old `data/` or `config/` directory over the new version. Keep independent backups of user projects; cross-version project compatibility has not been verified.

Network downloads require explicit permission for the relevant operation.

## Preview status and feedback

The portable package has been checked after extraction to a path containing Chinese characters and spaces, with development environment overrides removed. CLI commands, visible desktop startup/shutdown and application-local runtime loading passed on the packaging machine. A clean Windows environment and all asset workflows have not been fully validated. Complete skeleton binding is required for animation FBX/glTF exports.

Please [open an issue](https://github.com/girlgg/QCoDex-Releases/issues) with the QCoDex version, Windows version, GPU/driver, reproduction steps and full error message. Include a relevant screenshot when useful.

## Third-party components

Original third-party terms are included under `licenses/` in the portable package and are accessible in the About dialog. See [third-party information](THIRD-PARTY-NOTICES.md).
