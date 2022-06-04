# shvulkan library walkthrough

<button class="btn">[back to docs](./index)</button>

Setup
* [Clone and build](#clone-and-build)

Tutorial
* [CMake targets](#cmake-targes)
* [Graphics example](#graphics-example)
* [Compute example](#compute-example)

---

## Clone and Build

Open the terminal and run the following commands:
```bash
git clone --recursive https://github.com/MrSinho/shvulkan.git
cd shvulkan
mkdir build
cd build
cmake -DSH_VULKAN_BUILD_EXAMPLE=ON ..
cmake --build .
```

If you are having some trouble with building the targets and compiling the code, check the [Linux](https://github.com/MrSinho/shvulkan/blob/main/.shci/linux-log.md) and [Windows](https://github.com/MrSinho/shvulkan/blob/main/.shci/windows-log.md) build [logs](https://github.com/MrSinho/shvulkan/blob/main/.shci).

---

## CMake targets

| CMake target                                           | type       |
|--------------------------------------------------------|------------|
| [shvulkan](../ShVulkan/index)                       	 | library    |
| [shvulkan-graphics-example](#graphics-example)         | executable |
| [shvulkan-compute-example](#compute-example)           | executable |

If the cmake option `SH_VULKAN_BUILD_EXAMPLE` is enabled, the additional [`glfw`](https://github.com/glfw/glfw) target will be generated as a static library.

## Graphics example


---

## Compute example

---

<button class="btn">[top](#gaia-universe-model-library-walkthrough)</button>
<button class="btn">[back to docs](./index.md)</button>
 
---