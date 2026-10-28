# QCoDex

[简体中文](README.zh-CN.md)

QCoDex is a Windows x64 workbench for browsing, previewing and exporting supported game assets. This repository provides binary releases and usage information.

## Download

**[Download QCoDex v0.5.0 for Windows x64](https://github.com/girlgg/QCoDex-Releases/releases/download/v0.5.0/QCoDex-0.5.0-windows-x64.zip)** · [Release notes and checksums](https://github.com/girlgg/QCoDex-Releases/releases/tag/v0.5.0)

Version 0.5.0 is the first public preview. Download the program ZIP, not GitHub's automatically generated **Source code** archives. The separate Qt sources archive is for third-party source availability and rebuilding Qt; it is not required to run QCoDex.

## Requirements and first run

- Windows 11 x64 and a GPU/driver supporting Vulkan 1.3 and the required device features.
- Extract the **entire** ZIP to a folder writable by your account, then run `QCoDex.exe`.
- Qt, the VC++ runtime and application dependencies are bundled. No separate Qt, VC++ Redistributable or development SDK installation is required.
- Select your own game installation when you want to browse assets. The workbench can open without a registered game; game assets are not included.

The program provides asset browsing and search, image/model/material previews, model exports to CAST/FBX/glTF, image exports to PNG/DDS, and supported audio exports to WAV/FLAC. Available operations depend on the actual source format, asset type and required data. English and Simplified Chinese interfaces, light/dark themes and CLI commands are included. Run `QCoDex.exe --help` for CLI usage.

## Data and upgrades

Settings, caches and user documents default to `data/` beside the executable. Do not move the EXE on its own. Before upgrading, close all QCoDex instances and back up the **complete** `data/` directory. Extract the new version to a new folder before transferring your preserved data.

Network downloads require explicit permission for the relevant operation.

## Preview status and feedback

The portable package has been checked after extraction to a path containing Chinese characters and spaces, with development environment overrides removed. CLI commands, visible desktop startup/shutdown and application-local runtime loading passed on the packaging machine. A clean Windows environment and all asset workflows have not been fully validated. Complete skeleton binding is required for animation FBX/glTF exports.

Please [open an issue](https://github.com/girlgg/QCoDex-Releases/issues) with the QCoDex version, Windows version, GPU/driver, reproduction steps and full error message. Include a relevant screenshot when useful.

## Third-party components

Original third-party terms are included under `licenses/` in the portable package and are accessible in the About dialog. Corresponding Qt sources, local Qt changes and rebuild instructions are supplied as a separate release asset. See [third-party information](THIRD-PARTY-NOTICES.md).
