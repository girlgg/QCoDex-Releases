# QCoDex

[English](README.md)

QCoDex 是面向 Windows x64 的游戏资源浏览、预览与导出工作台。本仓库提供程序发布版和使用说明。

## 下载

**[下载 QCoDex v0.5.1 Windows x64 便携包](https://github.com/girlgg/QCoDex-Releases/releases/download/v0.5.1/QCoDex-0.5.1-windows-x64.zip)** · [版本说明](https://github.com/girlgg/QCoDex-Releases/releases/tag/v0.5.1)

`0.5.1` 为公开预览版更新。[详细更新说明](release-notes/0.5.1.zh-CN.md)。请下载程序 ZIP，不要下载 GitHub 自动生成的 **Source code** 压缩包。

## 系统要求与首次运行

- Windows 11 x64，以及支持 Vulkan 1.3 和所需设备功能的显卡与驱动。
- 将 ZIP **完整解压**到当前用户可写的目录，再运行 `QCoDex.exe`。
- Qt、VC++ 运行库及程序依赖均随包提供，无需另装 Qt、VC++ 运行库或开发 SDK。
- 浏览资源时选择自己的游戏安装目录。未登记游戏也可以打开界面，包内不包含游戏资产。

程序提供资源浏览与搜索、图像／模型／材质预览、CAST／FBX／glTF 模型导出、PNG／DDS 图像导出，以及受支持音频的 WAV／FLAC 导出。具体能力取决于实际来源格式、资产类型和所需数据。界面支持简体中文与英文、浅色与深色主题，并提供 CLI；命令行用法见 `QCoDex-Cmd.exe --help`。

## 数据与升级

0.5.1 预览版将配置保存在 EXE 同级 `config/`，数据库、缓存和用户文档默认保存在 `data/`。请备份完整旧程序目录，在新的可写目录解压新版。旧设置、安装登记、词库和目录库不迁移，不要用旧 `data/` 或 `config/` 覆盖新版。用户工程保留独立备份，本次未验证其跨版本兼容性。

联网下载须由具体操作明确允许。

## 预览版状态与反馈

程序包已在含中文和空格的路径下解压，并在清理开发环境变量后完成 CLI、可见桌面启动／退出和包内运行库加载检查。尚未在全新 Windows 环境和所有资源工作流中完成全面验收。动画 FBX／glTF 导出需要完整、有效的模型骨架绑定。

遇到问题请[提交 Issue](https://github.com/girlgg/QCoDex-Releases/issues)，附上 QCoDex 版本、Windows 版本、显卡与驱动、复现步骤和完整错误信息；必要时附界面截图。

## 第三方组件

第三方原始条款位于程序包 `licenses/`，也可在关于页查看。详见[第三方组件说明](THIRD-PARTY-NOTICES.md)。
