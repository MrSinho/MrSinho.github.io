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
cd Gaia_Universe_Model
mkdir build
cd build
cmake ..
cmake --build .
```

If you are having errors building the targets, check the [Linux](https://github.com/MrSinho/shvulkan/blob/main/.shci/linux-log.md) and [Windows](https://github.com/MrSinho/shvulkan/blob/main/.shci/windows-log.md) build [logs](https://github.com/MrSinho/shvulkan/blob/main/.shci).

## CMake targets

| CMake target                                           | type       |
|--------------------------------------------------------|------------|
| [shvulkan](../ShVulkan/index)                       	 | library    |
| [shvulkan-graphics-example](#graphics-example)         | executable |
| [shvulkan-compute-example](#compute-example)           | executable |

Inside the cloned repository directory download the GEDR3 binaries by executing one of the scripts shown below: 
```bash
#For Linux devices
./download_resources.sh
#For Windows devices
./download_resources.bat
```

## Graphics example

`gaia-universe-model-simulation` is a real time simulation, thus it needs all the libraries written on the table above.

## Compute example
```c

```

<button class="btn">[top](#gaia-universe-model-library-walkthrough)</button>
<button class="btn">[back to docs](./index.md)</button>
