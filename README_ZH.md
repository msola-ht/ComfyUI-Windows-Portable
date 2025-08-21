<div align="center">
ComfyUI-Windows-Portable
</div>


##

<div align="center">
  <a href="https://space.bilibili.com/1313066">Bilibili</a> ·
  <a href="https://www.youtube.com/@lunare-mcn">Youtube</a> ·
  <a href="https://github.com/msola-ht/ComfyUI-Windows-Portable">Text tutorial</a> ·
  <a href="https://pan.quark.cn/s/248b41dd8ee1">CN-Cloud disk address</a> 。
  <a href="https://huggingface.co/hemcn/ComfyUI-Portable/tree/main">Huggingface</a> 。
</div>


####

<div align="center">
  <a href="./README_ZH.md"><img src="https://img.shields.io/badge/简体中文-d9d9d9"></a>
  <a href="./README.md"><img src="https://img.shields.io/badge/English-d9d9d9"></a>
  <a href="./README_RU.md"><img src="https://img.shields.io/badge/Русский-d9d9d9"></a>
  <a href="./README_FR.md"><img src="https://img.shields.io/badge/Français-d9d9d9"></a>
  <a href="./README_DE.md"><img src="https://img.shields.io/badge/Deutsch-d9d9d9"></a>
  <a href="./README_JA.md"><img src="https://img.shields.io/badge/日本語-d9d9d9"></a>
  <a href="./README_KO.md"><img src="https://img.shields.io/badge/한국어-d9d9d9"></a>
  <a href="./README_AR.md"><img src="https://img.shields.io/badge/العربية-d9d9d9"></a>
  <a href="./README_ES.md"><img src="https://img.shields.io/badge/Español-d9d9d9"></a>
  <a href="./README_PT.md"><img src="https://img.shields.io/badge/Português-d9d9d9"></a>
</div>


##

## 整合包介绍以及说明：

### 环境配置说明

本整合包的构建与测试环境基于 **Miniforge3-25.1.1**，并使用其内置的 **Python 3.11** 版本创建 `venv` 虚拟环境。核心深度学习库配置如下：

- **PyTorch**: `2.7.1` (CUDA 12.8)
- **xformers**: `0.0.32+35bfb516.d20250730` (自编译版本)
- **triton-windows**: `3.3.1.post19`
- **sageattention**: `2.2.0+cu128torch2.7.1.post2`
- **Apex**: 自编译版本

### Windows 系统必备安装说明 (Windows System Prerequisites)

为确保本项目在 Windows 环境下顺利运行及相关组件的正确编译，请按照以下指南安装必备软件和驱动：

- **NVIDIA CUDA Toolkit 12.8.1**:
  - 为确保GPU加速功能及相关库（如 PyTorch、xformers、Apex）的兼容性与编译成功，强烈建议安装此特定版本。
  - 下载地址：[CUDA Toolkit 12.8.1](https://developer.nvidia.com/cuda-12-8-1-download-archive)
- **NVIDIA cuDNN 9.8.0.87**:
  - 深度学习库的关键加速组件。请确保其版本与您安装的 CUDA Toolkit 12.8.1 兼容，并按照官方指南正确配置（通常是将文件复制到 CUDA 安装目录）。
  - 下载地址：[cuDNN 9.8.0.87](https://developer.nvidia.com/cudnn-9-8-0-download-archive)
- **Conda 环境管理器 (版本 <= 25.1.1)**:
  - 推荐使用版本不高于 `25.1.1` 的 Conda 发行版（例如 Miniforge3 25.1.1 或 Anaconda/Miniconda 25.1.1）。
  - **重要提示**: 高于此版本的 Conda 可能会导致本项目提供的批处理脚本（`.bat` 文件）无法正确调用虚拟环境。
- **Visual Studio 2022**:
  - 用于编译本项目中需要从源代码构建的组件（如 `xformers` 和 `Apex`）。
  - 安装时请务必勾选 **“使用 C++ 的桌面开发” (Desktop development with C++)** 工作负载。
  - 下载地址：[Visual Studio 2022](https://visualstudio.microsoft.com/zh-hans/vs)

## 更新记录：

- 8-20：整合包分为国内版及全球版，除了启动文件不同，其他没有区别。

## 下载地址：

1. 中国下载：https://pan.quark.cn/s/248b41dd8ee1
2. 全球下载：https://huggingface.co/hemcn/ComfyUI-Portable/tree/main
