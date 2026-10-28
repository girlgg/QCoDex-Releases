# Third-party components

QCoDex's portable distribution includes third-party software and an embedded environment image. Their original notices and terms are preserved in the package's `licenses/` directory and are accessible through the About dialog. Publication of this repository does not relicense these components.

| Component | Version or identification | Terms and notices |
| --- | --- | --- |
| Qt | 6.12.0 shared libraries, QML modules and plugins | LGPLv3 and component-specific terms; `licenses/qt/` |
| Microsoft Visual C++ runtime | x64 MSVC v145 redistributable DLLs | Microsoft terms; `licenses/msvc/` |
| DirectXShaderCompiler | v1.9.2609 | Microsoft, MIT and LLVM notices; `licenses/dxc/` |
| Autodesk FBX SDK | 2020.3.7, with SDK-supplied static dependencies | Original SDK agreement and Autodesk statement; `licenses/fbxsdk/` |
| Oodle runtime | Oodle 8 Windows x64 | Proprietary component associated with RAD Game Tools / Epic Games Tools; supplied binary remains subject to its applicable terms |
| Opus / libFLAC | 1.5.2 / 1.5.0 | BSD-style and component terms; `licenses/audio/` |
| SPIRV-Tools / SPIRV-Headers / SPIRV-Reflect | Fixed versions used by this release | Apache-2.0 / MIT / Apache-2.0; `licenses/shader-compiler/` |
| Vulkan-Headers | 1.4.341 | Apache-2.0 OR MIT; `licenses/vulkan/` |
| nlohmann/json | 3.12.0 | MIT; `licenses/nlohmann-json/` |
| toml++ | 3.4.0 | MIT; `licenses/tomlplusplus/` |
| xxHash | 0.8.3 | BSD-2-Clause; `licenses/xxhash/` |
| SQLite | 3.50.2 | Public domain; `licenses/sqlite/` |
| bcdec | Fixed upstream header | MIT selection; `licenses/bcdec/` |
| Radiance decoder adaptation | image 0.25.10 source | MIT; `licenses/radiance/` |
| Additional format reference notice | Original retained notice | MIT; `licenses/notices/` |
| Studio Small 09 | Sergej Majboroda / Poly Haven, embedded 1k HDR | CC0; `licenses/environment/` |

## Qt sources and local changes

The `v0.5.0` release includes `QCoDex-0.5.0-qt-sources.zip`, containing the Qt source components used for the shared kit, the two local build patch recipes, pinned Vulkan-Headers input, original component licenses and independent Qt rebuild instructions. It is not required to run the portable program.

The kit applies a Vulkan declaration/build-path adjustment to Qt Quick and a swapchain acquisition-wait correction in Qt Gui. The changes are supplied in `patches/` in the source archive. Qt source files are provided with their original copyright and license notices.

Users can replace the shared Qt libraries with interface-compatible modified versions, retaining the required QML modules and plugins. Qt build tools, sources and development SDKs are not application startup requirements.

The component's original terms control where they differ from this summary. This repository does not assign a new common license to the program or its third-party components.
