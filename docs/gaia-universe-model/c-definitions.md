# gaia-universe-model C definitions

<button class="btn">[back to docs](./index)</button>

[Types and structures](#types-and-structures):
* Defined at [`gaiaUniverseModel.h`](https://github.com/MrSinho/gaia-universe-model/blob/main/gaia-universe-model/gaia-universe-model/include/gaia-universe-model/gaiaUniverseModel.h):
	* [GaiaUniverseModelMemory](#gaiauniversemodelmemory)
	* [GaiaModelDescriptorInfo](#gaiamodeldescriptorinfo)


[Functions](#functions):
* [gaiaReadModelDescriptor](#gaiareadmodeldescriptor)
* [gaiaReadSources](#gaiareadsources)
* [gaiaBuildPipeline](#gaiabuildpipeline)
* [gaiaWriteMemort](#gaiawritememory)
* [gaiaMemoryRelease](#gaiamemoryrelease)

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---



# Types and structures

## GaiaUniverseModelMemory
```c
typedef struct GaiaUniverseModelMemory {
	uint32_t			used_gpu_heap;
	void*				p_celestial_bodies;
	uint32_t			celestial_body_size;
	uint32_t			max_buffer_memory;
	uint32_t			available_video_memory;
	ShVkPipeline*		p_pipeline;
	ShVkFixedStates*	p_fixed_states;
} GaiaUniverseModelMemory;
```
### Description
Structure used to handle the universe model data when running the simulation. Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---

## GaiaModelDescriptorInfo
```c
typedef struct GaiaModelDescriptorInfo {
	uint32_t source_start;
	uint32_t source_end;
} GaiaModelDescriptorInfo;
```
### Description
Stores the universe model descriptor file located at [`gaia-universe-model/gaia-universe-model/assets/descriptors/universe-model.json`](https://github.com/MrSinho/gaia-universe-model/blob/main/gaia-universe-model/gaia-universe-model/assets/descriptors/universe-model.json). Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---



# Functions and macros

## gaiaReadModelDescriptor
```c
extern uint8_t gaiaReadModelDescriptor(const char* path, GaiaModelDescriptorInfo* p_descriptor_info);
```
### Description
Reads the universe model descriptor file located at [`gaia-universe-model/gaia-universe-model/assets/descriptors/universe-model.json`](https://github.com/MrSinho/gaia-universe-model/blob/main/gaia-universe-model/gaia-universe-model/assets/descriptors/universe-model.json). Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

### Parameters
 * **`path`**: valid [`gaia-universe-model/gaia-universe-model/assets/descriptors/universe-model.json`](https://github.com/MrSinho/gaia-universe-model/blob/main/gaia-universe-model/gaia-universe-model/assets/descriptors/universe-model.json) path;
 * **`descriptor_info`**: valid pointer to a [`GaiaModelDescriptorInfo`](#gaiamodeldescriptorinfo) structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>

int main(void) {
	GaiaModelDescriptorInfo descriptor_info = { 0 };

	gaiaError(
		gaiaReadModelDescriptor(path, &descriptor_infno) == 0,
		return 0;
	);

	//[...]
	return 1;
}


```

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---

## gaiaReadSources
```c
extern uint8_t gaiaReadSources(ShEngine* p_engine, const GaiaCelestialBodyFlags celestial_body_flags, const GaiaModelDescriptorInfo descriptor_info, GaiaUniverseModelMemory* p_model);
```
### Description
Reads the Universe Model source files. The amount of data read by the program depends on how much VRAM is not used by other processes. Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * **`celestial_body_flags`**: a [GaiaCelestialBodyFlags](../gaia-archive-tools/c-definitions.md#gaiacelestialbodyflags) value used to sort the data to read, by default equal to `GAIA_RA | GAIA_DEC | GAIA_BARYCENTRIC_DISTANCE | GAIA_TEFF`;
 * **`descriptor_info`**: [`GaiaModelDescriptorInfo`](#gaiamodeldescriptorinfo) structure;
 * **`p_universe_model`**: valid pointer to a [`GaiaUniverseModelMemory`](#gaiauniversemodelmemory) structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>

int main(void) {
	//setup engine
	//read model descriptor
	GaiaUniverseModelMemory model = { 0 };
	//read sources

	GaiaCelestialBodyFlags celestial_body_flags = GAIA_RA | GAIA_DEC | GAIA_BARYCENTRIC_DISTANCE | GAIA_TEFF;

	gaiaError(
		gaiaReadSources(&engine, celestial_body_flags, &model) == 0,
		return 0;
	);

	//[...]
	return 1;
}


```

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---


## gaiaBuildPipeline
```c
extern uint8_t gaiaBuildPipeline(ShEngine* p_engine, GaiaUniverseModelMemory* p_model);
```
### Description
Creates a graphics pipeline for rendering the celestial bodies. Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * **`GaiaUniverseModelMemory`**: valid pointer to a [`GaiaUniverseModelMemory`](#gaiauniversemodelmemory) structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>

int main(void) {
	//setup engine
	//read model descriptor
	GaiaUniverseModelMemory model = { 0 };
	//read sources

	gaiaError(
		gaiaBuildPipeline(&engine, &model) == 0,
		return 0;
	);

	//[...]
	return 1;
}

```

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---


## gaiaWriteMemory
```c
extern uint8_t gaiaWriteMemory(ShEngine* p_engine, GaiaUniverseModelMemory* p_model);
```
### Description
Writes universe model data on the GPU. Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

### Parameters
 * **`p_engine`**: valid pointer to an `ShEngine` structure;
 * **`p_universe_model`**: valid pointer to a [`GaiaUniverseModelMemory`](#gaiauniversemodelmemory) structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>

int main(void) {
	//setup engine
	//read model descriptor
	GaiaUniverseModelMemory model = { 0 };
	//read sources
	//build pipeline

	gaiaError(
		gaiaWriteMemory(&engine, &model) == 0,
		return 0;
	);

	//[...]
	return 1;
}

```

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---


## gaiaMemoryRelease
```c
#define gaiaMemoryRelease(p_universe_model)\
	free((p_universe_model)->p_celestial_bodies)\
```
### Description
Clears `p_universe_model->p_celestial_bodies` memory. Returns 1 if the operation completed successfully, otherwise the return value is equal to 0.

### Parameters
 * **`p_universe_model`**: valid pointer to a [`GaiaUniverseModelMemory`](#gaiauniversemodelmemory) structure.

### Usage example
```c
#include <gaia-universe-model/gaiaUniverseModel.h>

int main(void) {
	//setup engine
	//read model descriptor
	GaiaUniverseModelMemory model = { 0 };

	//read sources
	//build pipeline

	//[...]

	gaiaError(
		gaiaMemoryRelease(&model) == 0,
		return 0;
	);

	//[...]
	return 1;
}
```

<button class="btn">[top](#gaia-universe-model-c-definitions)</button>

---



<button class="btn">[top](#gaia-universe-model-c-definitions)</button>
<button class="btn">[back to docs](./index)</button>
