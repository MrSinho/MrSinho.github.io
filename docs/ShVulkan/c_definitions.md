# shvulkan C Definitions

<button>[back to index](./index.md)</button>

[Types and structures](#types-and-structures):
* Defined at [`shVkCore.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCore.h)
    * [ShVkCore](shvkcore)
    * [ShVkSurface](#shvksurface)
    * [ShVkQueue](#shvkqueue)
    * [ShVkCommand](#shvkcommand)
* Defined at [`shVkPipelineData.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkPipelineData.h)
    * [ShVkPipeline](#shvkpipeline)
    * [ShFixedStatesFlags](#shvkfixedstatesflags)
    * [ShVkFixedStates](#shvkfixedstates)

[Functions and macros](#functions):
* Defined at [`shVkCheck.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCheck.h):
    * [shCheckValidationLayers](#shcheckvalidationlayers)
    * [shTranslateVkResult](#shtranslatevkresult)
    * [shVkAssertResult](#shvkassertresult)
    * [shVkCheckResult](#shvkcheckresult)
* Defined at [`shVkCore.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCore.h)
    * [shCreateInstance](#shcreateinstance)
    * [shGetSurfaceCapabilities](#shgetsurfacecapabilities)
    * [shSelectPhysicalDevice](#shselectphysicaldevice)
    * [shSetQueueInfo](#shsetqueueinfo)
    * [shSetLogicalDevice](#shsetlogicaldevice)
    * [shCreateSwapchain](#shcreateswapchain)
    * [shGetSwapchainImages](#shgetswapchainimages)
    * [shCreateImageView](#shcreateimageview)
    * [shCreateSwapchainImageViews](#shcreateswapchainimageviews)
    * [shCreateCmdPool](#shcreatecmdpool)
    * [shCreateCmdBuffer](#shcreatecmdbuffer)
    * [shCreateCommandData](#shcreatecommanddata)
    * [shCreateRenderPass](#shcreaterenderpass)
    * [shSetFramebuffers](#shsetframebuffers)
    * [shSetSyncObjects](#shsetsyncobjects)
    * [shSwapchainRelease](#shswapchainrelease)
    * [shDepthBufferRelease](#shdepthbufferrelease)
    * [shSurfaceRelease](#shsurfacerelease)
    * [shCmdRelease](#shcmdrelease)
    * [shRenderPassRelease](#shrenderpassrelease)
    * [shInstanceRelease](#shinstancerelease)
    * [shVulkanRelease](#shvulkanrelease)
    * [shGetGraphicsQueue](#shgetgraphicsqueue)
    * [shGetComputeQueue](#shgetcomputequeue)
    * [shInitSwapchainData](#shinitswapchaindata)
    * [shCreateDepthImageView](#shcreatedepthimageview)
    * [shCreateGraphicsCommandBuffers](#shcreategraphicscommandbuffers)
    * [shCreateComputeCommandBuffers](#shcreatecomputecommandbuffers)
    * [shResetCommandBuffer](#shresetcommandbuffer)
    * [shResetFences](#shresetfences)
    * [shResetFence](#shresetfence)
    * [shBeginCommandBuffer](#shbegincommandbuffer)
    * [shQueueSubmit](#shqueuesubmit)
    * [shCmdDispatch](#shcmddispatch)
    * [shWaitForFences](#shwaitforfences)
    * [shWaitForFence](#shwaitforfence)
    * [shEndCommandBuffer](#shendcommandbuffer)
* Defined at [`shVkMemoryInfo.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkMemoryInfo.h)
    * [shCreateBuffer](#shcreatebuffer)
    * [shGetMemoryType](#shgetmemorytype)
    * [shAllocateMemory](#shallocatememory)
    * [shBindMemory](#shbindmemory)
    * [shReadMemory](#shreadmemory)
    * [shWriteMemory](#shwritememory)
    * [shClearBufferMemory](#shclearbuffermemory)
    * [shCreateImage](#shcreateimage)
    * [shGetMemoryBudgetProperties](#shgetmemorybudgetproperties)
    * [shCreateVertexBuffer](#shcreatevertexbuffer)
    * [shAllocateVertexBufferMemory](#shallocatevertexbuffermemory)
    * [shBindVertexBufferMemory](#shbindvertexbuffermemory)
    * [shWriteVertexBufferMemory](#shwritevertexbuffermemory)
    * [shBindVertexBuffer](#shbindvertexbuffer)
    * [shCreateIndexBuffer](#shcreateindexbuffer)
    * [shAllocateIndexBufferMemory](#shallocateindexbuffermemory)
    * [shBindIndexBufferMemory](#shbindindexbuffermemory)
    * [shWriteIndexBufferMemory](#shwriteindexbuffermemory)
    * [shBindIndexBuffer](#shbindindexbuffer)
    * [shClearVertexBufferMemory](#shclearvertexbuffermemory)
    * [shClearIndexBufferMemory](#shclearindexbuffermemory)
    * [shPipelineAllocateDescriptorBufferMemory](#shpipelineallocatedescriptorbuffermemory)
    * [shPipelineBindDescriptorBufferMemory](#shpipelinebinddescriptorbuffermemory)
    * [shPipelineClearDescriptorBufferMemory](#shpipelinecleardescriptorbuffermemory)
    * [shCreateDepthImage](#shcreatedepthimage)
    * [shInitDepthData](#shinitdepthdata)
* Defined at [`shVkPipelineData.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkPipelineData.h)
    * [shCreateRasterizer](#shcreaterasterizer)
    * [shSetMultisampleState](#shsetmultisamplestate)
    * [shColorBlendSettings](#shcolorblendsettings)
    * [shSetViewport](#shsetviewport)
    * [shSetFixedStates](#shsetfixedstates)
    * [shSetVertexInputAttribute](#shsetvertexinputattribute)
    * [shSetVertexInputState](#shsetvertexinputstate)
    * [shCreateInputAssembly](#shcreateinputassembly)
    * [shSetPushConstants](#shsetpushconstants)
    * [shCreateDescriptorBuffer](#shcreatedescriptorbuffer)
    * [shCreateDescriptorPool](#shcreatedescriptorpool)
    * [shDescriptorSetLayout](#shdescriptorsetlayout)
    * [shAllocateDescriptorSet](#shallocatedescriptorset)
    * [shCreateShaderModule](#shcreateshadermodule)
    * [shCreateShaderStage](#shcreateshaderstage)
    * [shSetupGraphicsPipeline](#shsetupgraphicspipeline)
    * [shSetupComputePipeline](#shsetupcomputepipeline)
    * [shEndPipeline](#shendpipeline)
    * [shPipelineRelease](#shpipelinerelease)
    * [shPipelineCreateDescriptorBuffer](#shpipelinecreatedescriptorbuffer)
    * [shPipelineCreateDynamicDescriptorBuffer](#shpipelinecreatedynamicdescriptorbuffer)
    * [shPipelineAllocateDescriptorBuffersMemory](#shpipelineallocatedescriptorbuffersmemory)
    * [shPipelineDescriptorSetLayout](#shpipelinedescriptorsetlayout)
    * [shPipelineCreateDescriptorPool](#shpipelinecreatedescriptorpool)
    * [shPipelineAllocateDescriptorSet](#shpipelineallocatedescriptorset)
    * [shPipelineCreateShaderStage](#shpipelinecreateshaderstage)
    * [shPipelineCreateShaderModule](#shpipelinecreateshadermodule)
    * [shPipelineWriteDescriptorBufferMemory](#shpipelinewritedescriptorbuffermemory)
    * [shPipelineWriteDynamicDescriptorBufferMemory](#shpipelinewritedynamicdescriptorbuffermemory)
    * [shPipelinePushConstants](#shpipelinepushconstants)
    * [shBindPipeline](#shbindpipeline)
    * [shPipelineUpdateDescriptorSets](#shpipelineupdatedescriptorsets)
    * [shPipelineUpdateDescriptorSet](#shpipelineupdatedescriptorset)
    * [shPipelineBindDescriptorSet](#shpipelinebinddescriptorset)
    * [shPipelineBindDescriptorSets](#shpipelinebinddescriptorsets)
    * [shPipelineBindDynamicDescriptorSet](#shpipelinebinddynamicdescriptorset)
    * [shPipelineBindDynamicDescriptorSets](#shpipelinebinddynamicdescriptorsets)
* Defined at [`shVkDescriptorStructureMap.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkDescriptorStructureMap.h)
    * [SH_VULKAN_GENERATE_DESCRIPTOR_STRUCTURE_MAP](#sh_vulkan_generate_descriptor_structure_map)
* Defined at [`shVkDrawLoop.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkDrawLoop.h)
    * [shFrameReset](#shframereset)
    * [shFrameBegin](#shframebegin)
    * [shDrawIndexed](#shdrawindexed)
    * [shDraw](#shdraw)
    * [shFrameEnd](#shframeend)



---



# Types and structures



## ShVkCore
```c
typedef struct ShVkCore {
	VkInstance							instance;
	VkPhysicalDevice					physical_device;
	VkPhysicalDeviceProperties			physical_device_properties;
	VkPhysicalDeviceFeatures			physical_device_features;
	VkPhysicalDeviceMemoryProperties	physical_device_memory_properties;
	VkDevice							device;
	ShVkSurface							surface;
	VkQueueFlags						required_queue_flags;
	ShVkQueue							graphics_queue;
	ShVkQueue							compute_queue;
	uint32_t							thread_count;
	ShVkCommand*						p_graphics_commands;
	ShVkCommand*						p_compute_commands;
	VkSwapchainKHR						swapchain;
	VkFormat							swapchain_image_format;
	uint32_t							swapchain_image_count;
	VkImage*							p_swapchain_images;
	VkImageView*						p_swapchain_image_views;
	VkFramebuffer*						p_frame_buffers;
	VkImage								depth_image;
	VkDeviceMemory						depth_image_memory;
	VkImageView							depth_image_view;
	VkRenderPass						render_pass;
	VkSemaphore*						p_render_semaphores;
} ShVkCore;
```
### Description
Primary handle for the Vulkan API context and devices. Stores unique buffers (framebuffers, depth buffer), graphics and compute command buffers, and thread synchronization structures.

---

## ShVkSurface
```c
typedef struct ShVkSurface {
	VkSurfaceKHR				surface;
	uint32_t					width;
	uint32_t					height;
	VkSurfaceCapabilitiesKHR	surface_capabilities;
} ShVkSurface;
```
### Description
Collection of [`VkSuraceKHR`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkSurfaceKHR.html), surface width, height and other specific properties.

---

## ShVkQueue
```c
typedef struct ShVkQueue {
	uint32_t		queue_family_index;
	VkQueue			queue;
} ShVkQueue;
```
### Description
Stores the queue family index of a specific [`VkQueue`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkQueue.html).

---

## ShVkCommand
```c
typedef struct ShVkCommand {
	VkCommandBuffer cmd_buffer;
	VkCommandPool	cmd_pool;
	VkFence			fence;
} ShVkCommand;
```
### Description
A thread unit: stores a [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), the relative [`VkCommandPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandPool.html) and [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html) for thread synchronization.

---

## ShVkPipeline
```c
typedef struct ShVkPipeline {
	uint32_t							shader_module_count;
	VkShaderModule						shader_modules[16];
	VkPipelineShaderStageCreateInfo		shader_stages[16];
	VkPushConstantRange					push_constant_range;
	uint32_t							descriptor_count;
	VkBuffer							descriptor_buffers[32];
	VkDescriptorSetLayout				descriptor_set_layouts[32];
	VkDescriptorSet						descriptor_sets[32];
	VkWriteDescriptorSet				write_descriptor_sets[32];
	VkDeviceMemory						descriptor_buffers_memory[32];
	VkDescriptorSetLayoutBinding		descriptor_set_layout_bindings[32];
	VkDescriptorBufferInfo				descriptor_buffer_infos[32];
	VkDescriptorPool					descriptor_pools[32];
	uint32_t							dynamic_descriptor_buffer_offsets[32];
	VkPipelineLayout					pipeline_layout;
	VkPipeline							pipeline;
} ShVkPipeline;
```
### Description
The pipeline handle. It holds the shader modules along with shader input-output parameters. To setup a graphics pipeline, use [shVkSetupGraphicsPipeline](#shvksetupgraphicspipeline), while [shVkSetupComputePipeline](#shvksetupcomputepipeline) for compute purposes.

---

## ShVkFixedStatesFlags
```c
typedef enum ShVkFixedStateFlags  {
	SH_FIXED_STATES_POLYGON_MODE_WIREFRAME				= 0b000000001,
	SH_FIXED_STATES_POLYGON_MODE_FACE					= 0b000000010,
	SH_FIXED_STATES_POLYGON_MODE_POINTS					= 0b000000100,
	SH_FIXED_STATES_PRIMITIVE_TOPOLOGY_TRIANGLE_LIST	= 0b000001000,
	SH_FIXED_STATES_PRIMITIVE_TOPOLOGY_LINE_LIST		= 0b000010000,
	SH_FIXED_STATES_PRIMITIVE_TOPOLOGY_POINT_LIST		= 0b000100000,
} ShVkFixedStateFlags;
```
### Description
Some setup flags required when creating a graphics pipeline (see [shVkSetupGraphicsPipeline](#shvksetupgraphicspipeline)).

---

## ShVkFixedStates
```c
typedef struct ShVkFixedStates {
	VkVertexInputBindingDescription			vertex_binding_description;
	uint32_t								vertex_input_attribute_description_count;
	VkVertexInputAttributeDescription		vertex_input_attributes[32];
	VkPipelineVertexInputStateCreateInfo	vertex_input_state_info;
	VkPipelineInputAssemblyStateCreateInfo	input_assembly;
	VkViewport								viewport;
	VkRect2D								scissor;
	VkPipelineViewportStateCreateInfo		viewport_state;
	VkPipelineRasterizationStateCreateInfo	rasterizer;
	VkPipelineColorBlendAttachmentState		color_blend_attachment;
	VkPipelineColorBlendStateCreateInfo		color_blend_state;
	VkPipelineMultisampleStateCreateInfo	multisample_state_info;
	ShVkFixedStateFlags 					fixed_state_flags;
} ShVkFixedStates;
```
### Description
Defines some fixed pre-rendering steps and image processing operations when dealing with graphics pipelines.

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