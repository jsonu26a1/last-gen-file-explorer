Development Environment Setup
=============================

_**this document is a work in progress**_

Development will take place in VS Code on Windows. First, you will need the MSVC tools installed.

## 1. Install MSVC

This document covers two ways, 1. requires less disk space, and 2. just installs the entire Visual Studio IDE. You can skip this step if you already have MSVC installed.

### 1. Install Build Tools for Visual Studio
This will require less disk space, but requires manually selecting certain "Individual components" within the "Visual Studio Installer". 

Go to the [Visual Studio download page](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022), and click on the download button under the section "Build Tools for Visual Studio 2022".
This specific "Visual Studio Installer" is needed to avoid installing the full VS IDE by default.

The installer will have tabs for "Workloads", "Individual components", "Language packs", and "Installation locations". Under the "Individual components" tab, select/check the following components in each category:

- **Compilers, build tools, and runtimes**
  - "C++ CMake tools for Windows"
  - "C++ 2022 Redistributable Update"
  - "MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest)"
    - (auto-selected as a dependency for "C++ CMake tools for Windows")
- **Development Activities**
  - "C++ Build Tools core features"
- **SDKs, libraries, and frameworks**
  - "Windows Universal C Runtime"
    - (auto-selected as a dependency for "C++ Build Tools core features")

Then click "Install"

### 2. Install Visual Studio
This is the easiest option, but requires more disk space because the VS IDE and other components will also be installed.

Go to the [Visual Studio download page](https://visualstudio.microsoft.com/downloads/), and download the installed (probably the "Community" edition, with the button labeled "Free download")

Under the "Workloads" tab, under the "Desktop & Mobile" section, select/check the "Desktop development with C++" item. Then click "Install"

## 2. Setting up VS Code

TODO: summarize these guides?
- https://code.visualstudio.com/docs/languages/cpp
- https://code.visualstudio.com/docs/cpp/config-msvc

TODO: test to make sure the "Install MSVC" steps are adequate for C++ development in vscode
