# shvulkan library

<button class="btn">[back to docs](./index)</button>

Setup
* [Clone and build](#clone-and-build)

Tutorial
* [Cmake targets](#cmake-targes)
* [Graphics example](#graphics-example)
* [Compute example](#compute-example)

---

# Setup

## Clone and Build

Open the terminal and run the following commands:
```bash
git clone --recursive https://github.com/MrSinho/Gaia_Universe_Model.git
cd Gaia_Universe_Model
mkdir build
cd build
cmake ..
cmake --build .
```

## Download Universe Model Data

Inside the cloned repository directory download the GEDR3 binaries by executing one of the scripts shown below: 
```bash
#For Linux devices
./download_resources.sh
#For Windows devices
./download_resources.bat
```

# Tutorial

## Use CMake

| CMake target                                           | type       |
|--------------------------------------------------------|------------|
| [shvulkan](../ShVulkan/index)                       | library    |
| [shengine](../ShEngine/index)                       | library    |
| [gaia-archive-tools](../Gaia_Archive_Tools/index)   | library    |
| [gaia-universe-model](../Gaia_Universe_Model/index) | library    |
| gaia-universe-model-simulation                         | executable |

`gaia-universe-model-simulation` is a real time simulation, thus it needs all the libraries written on the table above.

## Example
```c

```

<button class="btn">[top](#gaia-universe-model-library-walkthrough)</button>
<button class="btn">[back to docs](./index.md)</button>
