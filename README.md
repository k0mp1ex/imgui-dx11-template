# ImGui template for DX11 with CMake + VCPKG

Simple [Dear ImGui](https://github.com/ocornut/imgui) template to build with CMake using VCPKG linking against DirectX11 backend for easy prototype for folks that don't want to work with the Visual Studio solution that comes with the official examples.

The code in `main.cpp` is from the [official ImGui example](https://github.com/ocornut/imgui/blob/master/examples/example_win32_directx11/main.cpp).
This template uses the experimental `docking` features.

## What should I update in the template?

- the `LICENSE`
- the project name in `CMakelists.txt`
- the `name` and `version` in the `vcpkg.json`

## How to build and run?

The steps below are for `debug` preset. Change it to `release` when shipping your app and rename the last step with your executable name (it will match your project name).

1) Configure: `cmake --preset debug`
2) Build: `cmake --build build\debug --target ImGuiDx11Template`
3) Run: `cd build\debug && ImGuiDx11Template.exe`
