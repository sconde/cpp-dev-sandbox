# C++ Dev Sandbox

A Docker dev container for C/C++. Inspired by [C++ DevBox](https://github.com/jakoch/cpp-devbox/tree/main).

Forked from [cpp-dev-sandbox](https://github.com/vitaliy-ostapchuk93/cpp-dev-sandbox).

Build and tested with latest **Ubuntu (24.04 LTS)** with **GCC++ v.14**, **Clang v.18**, and **MSVC v.19.39.33523**.

Simple **CMake** project on **C++23** standard using **Modules**.

Cross-platform config defined using `CMakePresets.json`.

Optional package management with **vcpkg**.

*Note: This is a dev container! Consider using a dedicated runtime image and copy your artifacts there to have a clean & small image!*

## Fork Modifications

- **Integrated cppinsights:**
  - Installed `cppinsights` in `/opt` and added it to the PATH for easy access. This allows for deeper code analysis and insights into how C++ code is transformed during compilation.

- **Added support for C/C++ Compiler Explorer VS Code Extension:**
  - Configured the dev container to include the **C/C++ Compiler Explorer** extension. This enables interactive code exploration and visualization within VS Code.

## Usage

1. **Building the Docker Container:**

   ```sh
   docker build -t cpp-dev-sandbox .
