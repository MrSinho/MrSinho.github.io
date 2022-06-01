# Gaia Universe Model C Definitions

<button>[back to index](./index)</button>

[Types and structures](#types-and-structures):
* [GaiaUniverseModelMemory](#gaiauniversemodelmemory)

[Functions](#functions):
* [gaiaEngineSetup](#gaiaenginesetup)
* [gaiaSetupMaterial](#gaiasetupmaterial)
* [gaiaReadSources](#gaiareadsources)
* [gaiaWriteVertexBuffers](#gaiawritevertexbuffers)
* [gaiaSceneSetup](#gaiascenesetup)
* [gaiaSceneUpdate](#gaiasceneupdate)
* [gaiaMemoryRelease](#gaiamemoryrelease)
* [gaiaEngineShutdown](#gaiaengineshutdown)

---

# Types and structures


## GaiaUniverseModelMemory
```c
typedef struct GaiaUniverseModelMemory {
	ShMaterialHost	materials[1];
	uint32_t		used_vram;
	void*			p_celestial_bodies;
	uint32_t		vertex_buffer_count;
	VkBuffer		vertex_buffers[64];
	VkDeviceMemory	vertex_buffers_memory[64];
	void*			push_constant[128 / sizeof(void*)];
	void*			uniform_buffer[16 / sizeof(void*)];
} GaiaUniverseModelMemory;
```
### Description
Structure used to handle the Universe Model data.

---


# Functions


## gaiaEngineSetup
```c
void gaiaEngineSetup(ShEngine* p_engine);
```
### Description
Initializes the Vulkan engine and creates a glfw window.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure. 

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>

ShEngine engine = { 0 };
gaiaEngineSetup(&engine);
```
---


## gaiaSetupMaterial
```c
void gaiaSetupMaterial(ShEngine* p_engine, GaiaUniverseModelMemory* p_universe_model);
```
### Description
Creates a graphics pipeline for rendering the celestial bodies.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * [**`GaiaUniverseModelMemory`**](#gaiauniversemodelmemory): valid pointer to a `GaiaUniverseModelMemory` structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine first...
GaiaUniverseModelMemory universe_model = { 0 };
gaiaSetupMaterial(&engine, &universe_model);
```
---

## gaiaReadSources
```c
void gaiaReadSources(ShEngine* p_engine, const GaiaCelestialBodyFlags celestial_body_flags, GaiaUniverseModelMemory* p_universe_model);
```
### Description
Reads the Universe Model source files. The number of bytes read depends on how much VRAM is ready to be used.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * [**`celestial_body_flags`**](https://mrsinho.github.io/docs/Gaia_Archive_Tools/c_definitions.html#gaiacelestialbodyflags): used to choose what data to read;
 * [**`p_universe_model`**](#gaiauniversemodelmemory): valid pointer to a `GaiaUniverseModelMemory` structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine and material first
uint64_t celestial_body_flags = GAIA_RA | GAIA_DEC | GAIA_BARYCENTRIC_DISTANCE | GAIA_TEFF;
gaiaReadSources(&engine, celestial_body_flags, &universe_model);
```
---


## gaiaWriteVertexBuffers
```c
void gaiaWriteVertexBuffers(ShEngine* p_engine, GaiaUniverseModelMemory* p_universe_model);
```
### Description
Writes vertex buffer data on the GPU.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * [**`p_universe_model`**](#gaiauniversemodelmemory): valid pointer to a `GaiaUniverseModelMemory` structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine and material first, be sure to have read the source files
gaiaWriteVertexBuffers(&engine, &universe_model);
```
---

## gaiaSceneSetup
```c
gaiaSceneSetup(&engine);
```
### Description
Initializes the main scene. Required before rendering.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine first
void gaiaSceneSetup(ShEngine* p_engine);
```
---


## gaiaSceneUpdate
```c
void gaiaSceneUpdate(ShEngine* p_engine, GaiaUniverseModelMemory* p_universe_model);
```
### Description

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * [**`p_universe_model`**](#gaiauniversemodelmemory): valid pointer to a `GaiaUniverseModelMemory` structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine and material first
//Read source files and write vertex buffer memory
//Initialize scene

//Get size of a celestial body
uint64_t celestial_body_flags = GAIA_RA | GAIA_DEC | GAIA_BARYCENTRIC_DISTANCE | GAIA_TEFF;
const uint32_t CELESTIAL_BODY_SIZE = gaiaGetBodySize(celestial_body_flags);

while (shIsWindowActive(engine.window.window)) {
		//UPDATE WINDOW
		shUpdateWindow(&engine);

		//BEGIN FRAME
		shFrameReset(&engine.core);
		uint32_t frame_index = 0;
		shFrameBegin(&engine.core, &frame_index);

		//UPDATE SCENE AND START DRAWING
		gaiaSceneUpdate(&engine, &universe_model);
		shDraw(&engine.core, universe_model.used_vram / CELESTIAL_BODY_SIZE);

		//END FRAME
		shEndPipeline(&engine.p_materials[0].pipeline);
		shFrameEnd(&engine.core, frame_index);
	}
```
---


## gaiaMemoryRelease
```c
void gaiaMemoryRelease(ShEngine* p_engine, GaiaUniverseModelMemory* p_universe_model);
```
### Description
Frees universe model memory and vertex buffer buffer memory.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * [**`p_universe_model`**](#gaiauniversemodelmemory): valid pointer to a `GaiaUniverseModelMemory` structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine and material first
//Read source files and write vertex buffer memory
//End rendering
gaiaMemoryRelease(&engine, &universe_model);
```
---


## gaiaEngineShutdown
```c
void gaiaEngineShutdown(ShEngine* p_engine);
```
### Description
Clears uniform buffers, ends the graphics pipeline and releases every Vulkan structure. 

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>
//Setup engine and material first
//Read source files and write vertex buffer memory
//End rendering
//Clear vertex buffers
gaiaEngineShutdown(&engine);
```



---


<button>[back to index](./index)</button>
