# Third-party components

QCoDex's portable distribution includes third-party software and an embedded environment image. Their original notices and terms are preserved in the package's `licenses/` directory and are accessible through the About dialog. Publication of this repository does not relicense these components.

| Component | Version or identification | Terms and notices |
| --- | --- | --- |
| Qt | 6.12.0 shared libraries, QML modules and plugins | LGPLv3 and component-specific terms; `licenses/qt/` |
| Microsoft Visual C++ runtime | x64 MSVC v145 redistributable DLLs | Microsoft terms; `licenses/msvc/` |
| DirectXShaderCompiler | v1.9.2609 | Microsoft, MIT and LLVM notices; `licenses/dxc/` |
| Autodesk FBX SDK | 2020.3.7, with SDK-supplied static dependencies | Original SDK agreement and Autodesk statement; `licenses/fbxsdk/` |
| Oodle runtime | Oodle 8 Windows x64 | Proprietary component associated with RAD Game Tools / Epic Games Tools; supplied binary remains subject to its applicable terms |
| Opus / libFLAC | 1.5.2 / 1.5.0 | BSD-style and component terms; Opus: `licenses/audio/`; FLAC: `licenses/export/` |
| SPIRV-Tools / SPIRV-Headers / SPIRV-Reflect | Fixed versions used by this release | Apache-2.0 / MIT / Apache-2.0; `licenses/shader-compiler/` |
| Vulkan-Headers | 1.4.341 | Apache-2.0 OR MIT; `licenses/vulkan/` |
| Glaze | 9.1.0 | MIT; `licenses/glaze/` |
| OpenCV | 4.13.0, static core / imgproc / imgcodecs | Apache-2.0, retained BSD terms and SoftFloat / fdlibm notices; `licenses/opencv/` |
| libpng / zlib | 1.6.53 / 1.3.1, bundled through OpenCV | Original component licenses; `licenses/opencv/libpng/`, `licenses/opencv/zlib/` |
| Tracy | 0.14.1 static client | BSD-3-Clause; `licenses/tracy/` |
| LZ4 | 1.10.0 | BSD-2-Clause; `licenses/lz4/` |
| VulkanMemoryAllocator | 3.3.0 | MIT; `licenses/vma/` |
| xxHash | 0.8.3 | BSD-2-Clause; `licenses/xxhash/` |
| SQLite | 3.50.2 | Public domain; `licenses/sqlite/` |
| bcdec | Fixed upstream header | MIT selection; `licenses/bcdec/` |
| Radiance decoder adaptation | image 0.25.10 source | MIT; `licenses/radiance/` |
| Additional format reference notice | Original retained notice | MIT; `licenses/notices/` |
| Studio Small 09 | Sergej Majboroda / Poly Haven, embedded 1k HDR | CC0; `licenses/environment/` |

## Qt

The portable package uses shared Qt 6.12.0 libraries. Original component license texts are preserved under `licenses/qt/` in the package.

## Distribution scope

This list describes the 0.5.1 portable candidate. nlohmann/json and toml++ are no longer product dependencies. RenderDoc itself and the optional Tracy capture/report tools are not bundled. The RenderDoc SDK header and replay adapter notices are retained in `licenses/renderdoc/`; Tracy client terms remain in `licenses/tracy/`.
