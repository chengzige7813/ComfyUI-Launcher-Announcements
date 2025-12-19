# ComfyUI 启动器 ✨ 

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![PyQt6](https://img.shields.io/badge/PyQt6-6.0+-green.svg)
![License](https://img.shields.io/badge/License-商业授权-red.svg)

**让 ComfyUI 的启动体验变得更简单一些**

[功能介绍](#-功能介绍) • [开始使用](#-开始使用) • [开发计划](#-开发计划) • [问题反馈](#-遇到问题) • [联系方式](#-联系方式)

</div>

---

## 💭 写在前面

开发这个启动器是因为自己在用 ComfyUI 时，总觉得每次启动都要打开命令行窗口，配置各种参数，有时还会遇到网络问题。

作为一个经常使用 ComfyUI 的人，我想也许可以做个图形化的启动器，让日常使用更方便一些。 

---

## 🎉 功能介绍

### 简化启动流程 🚀
点击启动按钮就可以运行 ComfyUI，不需要手动打开命令行或配置参数。启动器会自动处理这些细节。

### 网络优化 ⚡
- 模型下载：内置了国内镜像源配置，可以使用预设，也可以使用自定义加速地址。
- 插件安装：集成了 GitHub 加速服务，但不是完全使用覆盖加速，
  - ✅ 会走镜像加速的操作：
    - git clone 克隆插件仓库
    - git pull 更新插件
    - 通过环境变量控制的下载
  ❌ 不走镜像的操作：
    - ComfyUI-Manager的插件列表API请求（aiohttp直连）
    - Manager的部分metadata请求
  但是因为comyui manager源码在获取更新列表还是硬编码了直链，部分更新可能受阻，但不影响使用。
- 代理设置：出现各种莫名其妙的连接失败和超时，可以配置自己的代理参数。

### 启动优化 
- 高级设置页：分为新手模式和开发者模式。
- 新手模式：已经配置了常用的预设，不需要额外的理解各种启动参数。
- 开发者模式：可以完全自定义参数，包括各种性能优化，内存优化，显存优化，自定义python解释器，Git解释器的路径。

### 版本更新 🔄
当 ComfyUI 有新版本时，可以在启动器里直接更新。前端、插件、依赖包都可以单独管理。

### 界面设计 🎨
使用深色主题，长时间使用会舒服一些。界面布局尽量保持简洁。

### 其他功能 💡
- 支持托盘模式，可以最小化到系统托盘，需要时再打开  
- 提供开机自启选项，适合每天都会用到的情况

---

## 🔮 开发计划

### 插件管理 🔥
正在开发插件管理功能，计划支持浏览、搜索、安装和卸载插件，以及自动处理依赖关系。

### 模型管理 🔥
也在考虑添加模型管理功能，比如查看模型信息、自动分类、检测重复文件等。如果能支持断点续传，网络不稳定时会好用很多。

### 其他想法
- 工作流模板库：可以保存和分享常用的工作流
- 多语言支持：考虑添加英文界面

如果你有什么想法或建议，欢迎在 Issues 里聊聊，我会认真考虑的。

---

## 🎮 开始使用

### 使用整合包 💝
如果你使用的是整合包，直接双击 `启动器.exe` 即可运行。

整合包中已经包含：
- ✅ 配置好的 Python 环境
- ✅ 一些常用的基础模型
- ✅ 预装了常见的插件
- ✅ 可以直接开始使用

---

## 😭 遇到问题

可以通过以下方式反馈问题：

**GitHub Issues**（推荐）  
→ [提交 Issue](https://github.com/chengzige7813/ComfyUI-cher-Package-Launcher/issues)

**Gitee Issues**（国内访问）  
→ [提交 Issue](https://gitee.com/chengzige7813/comfyui-cher-package-launcher/issues)

### 反馈时的建议 📝
如果能提供以下信息，会更容易定位问题：
- 操作系统版本（比如 Windows 10 或 11）
- Python 版本号
- 显卡型号
- 问题的具体表现，有截图或错误日志会更好
- 问题出现的步骤

详细的信息能帮助更快地解决问题。

---

## 💬 联系方式

### 作者信息 👋

- GitHub: [@chengzige7813](https://github.com/chengzige7813)
- Gitee: [@chengzige7813](https://gitee.com/chengzige7813)
- 邮箱: chengzige7813@outlook.com

### 关于整合包 💼

<div align="center">

![](https://raw.githubusercontent.com/meta10110/Picture_bed/main/images/chengzige7813.png)

*添加时备注"ComfyUI"哦～*

</div>

---

## ⚠️ 版权说明

本项目采用商业授权模式。

如需商业合作或源码授权，欢迎联系讨论。

---

## 🙏 感谢这些项目

- [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- [PyQt6](https://www.riverbankcomputing.com/software/pyqt/)

---

<div align="center">

## ⭐ 如果觉得有用

欢迎给项目点个 Star，这是对项目最好的支持。

![GitHub stars](https://img.shields.io/github/stars/chengzige7813/ComfyUI-cher-Package-Launcher?style=social)
![GitHub forks](https://img.shields.io/github/forks/chengzige7813/ComfyUI-cher-Package-Launcher?style=social)

---

Made with ❤️ by [chengzige7813](https://github.com/chengzige7813)

希望这个启动器能帮到你。

</div>
