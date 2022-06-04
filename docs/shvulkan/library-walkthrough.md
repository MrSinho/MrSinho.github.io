# shvulkan library walkthrough

<button class="btn">[back to docs](./index)</button>

Setup
* [Clone and build](#clone-and-build)

Tutorial
* [CMake targets](#cmake-targets)
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
cmake -DSH_VULKAN_BUILD_EXAMPLES=ON ..
cmake --build .
```

If you are having some trouble with building the targets and compiling the code, check the [Linux](https://github.com/MrSinho/shvulkan/blob/main/.shci/linux-log.md) and [Windows](https://github.com/MrSinho/shvulkan/blob/main/.shci/windows-log.md) build [logs](https://github.com/MrSinho/shvulkan/blob/main/.shci).

### Vulkan version
> Vulkan 1.3 updates are coming soon

If you haven't install Vulkan 1.2 you can set the cmake options `SH_USE_VULKAN_1_0` or `SH_USE_VULKAN_1_1` as true:
```bash
cmake -DSH_USE_VULKAN_1_0=ON ..
cmake -DSH_USE_VULKAN_1_1=ON ..
```

---

## CMake targets

| CMake target                                           | type       |
|--------------------------------------------------------|------------|
| [shvulkan](../ShVulkan/index)                       	 | library    |
| [shvulkan-graphics-example](#graphics-example)         | executable |
| [shvulkan-compute-example](#compute-example)           | executable |

If the cmake option `SH_VULKAN_BUILD_EXAMPLES` is enabled, the additional [`glfw`](https://github.com/glfw/glfw) target will be generated as a static library.

## Graphics example

the author is writing...
```c

```

---

## Compute example

the author is writing...
```c

```

---

<button class="btn">[top](#shvulkan-library-walkthrough)</button>
<button class="btn">[back to docs](./index.md)</button>
 
---