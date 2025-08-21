<div align="center">
ComfyUI-Windows-Portable
</div>



##

<div align="center">
  <a href="https://space.bilibili.com/1313066">Bilibili</a> ·
  <a href="https://www.youtube.com/@lunare-mcn">Youtube</a> ·
  <a href="https://github.com/msola-ht/ComfyUI-Windows-Portable">Text tutorial</a> ·
  <a href="https://pan.quark.cn/s/248b41dd8ee1">CN-Cloud disk address</a> .
  <a href="https://huggingface.co/hemcn/ComfyUI-Portable/tree/main">Huggingface</a> .
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
## Update Log:

- 8-20: The integrated package is divided into domestic and global versions, with no differences other than the startup files.

## About the Integrated Package and Instructions:

### Environment Configuration Instructions

This integrated package is built and tested based on **Miniforge3-25.1.1**, and uses its built-in **Python 3.11** version to create a `venv` virtual environment. The core deep learning library configuration is as follows:

- **PyTorch**: `2.7.1` (CUDA 12.8)
- **xformers**: `0.0.32+35bfb516.d20250730` (Self-compiled version)
- **triton-windows**: `3.3.1.post19`
- **sageattention**: `2.2.0+cu128torch2.7.1.post2`
- **Apex**: Self-compiled version

### Windows System Prerequisites

To ensure the smooth operation of the integrated package in a Windows environment and the correct compilation of related components, please install the necessary software and drivers according to the following guide:

**NVIDIA CUDA Toolkit 12.8.1**:
- To ensure compatibility and successful compilation of GPU acceleration features and related libraries (such as PyTorch, xformers, Apex), it is strongly recommended to install this specific version.
- Download address: [CUDA Toolkit 12.8.1](https://developer.nvidia.com/cuda-12-8-1-download-archive)

**NVIDIA cuDNN 9.8.0.87**:
- A key acceleration component for deep learning libraries. Please ensure its version is compatible with your installed CUDA Toolkit 12.8.1 and configure it correctly according to the official guide (usually by copying files to the CUDA installation directory).
- Download address: [cuDNN 9.8.0.87](https://developer.nvidia.com/cudnn-9-8-0-download-archive)

**Conda Environment Manager (version <= 25.1.1)**:
- It is recommended to use a Conda distribution no higher than `25.1.1` (e.g., Miniforge3 25.1.1 or Anaconda/Miniconda 25.1.1).
- **Important Note**: Conda versions higher than this may cause the batch scripts (`.bat` files) provided in this project to fail to correctly call the virtual environment.

**Visual Studio 2022**:
- Used for compiling components of the integrated package that need to be built from source (such as `xformers` and `Apex`).
- When installing, be sure to check the **"Desktop development with C++"** workload.
- Download address: [Visual Studio 2022](https://visualstudio.microsoft.com/zh-hans/vs)

### Built-in Nodes

-  [Nodes List](custom_nodes/en.md) 

## Download Addresses:

1. China Download: https://pan.quark.cn/s/248b41dd8ee1
2. Global Download: https://huggingface.co/hemcn/ComfyUI-Portable/tree/main
