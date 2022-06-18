# shvulkan C definitions

<button class="btn">[back to docs](./index)</button>

[Types and structures](#types-and-structures):
* Defined at [`shVkCore.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCore.h)
    * [ShVkCore](#shvkcore)
    * [ShVkSurface](#shvksurface)
    * [ShVkQueue](#shvkqueue)
    * [ShVkCommand](#shvkcommand)
    * [ShVkImageType](#shvkimagetype)
* Defined at [`shVkPipelineData.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkPipelineData.h)
    * [ShVkPipeline](#shvkpipeline)
    * [ShVkFixedStatesFlags](#shvkfixedstateflags)
    * [ShVkFixedStates](#shvkfixedstates)

[Functions and macros](#functions-and-macros):
* Defined at [`shVkCheck.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCheck.h):
    * [shCheckValidationLayers](#shcheckvalidationlayers)
    * [shTranslateVkResult](#shtranslatevkresult)
    * [shVkError](#shvkerror)
    * [shVkResultError](#shvkresulterror)
* Defined at [`shVkCore.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCore.h)
    * [shCreateInstance](#shcreateinstance)
    * [shSelectPhysicalDevice](#shselectphysicaldevice)
    * [shSetQueueInfo](#shsetqueueinfo)
    * [shSetLogicalDevice](#shsetlogicaldevice)
    * [shCreateSwapchain](#shcreateswapchain)
    * [shGetSwapchainImages](#shgetswapchainimages)
    * [shCreateSwapchainImageViews](#shcreateswapchainimageviews)
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
    * [shCreateDepthImageView](#shcreatedepthimageview)
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
    * [shDescriptorSetLayout](#shdescriptorsetlayout)
    * [shCreateDescriptorPool](#shcreatedescriptorpool)
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
    * [shPipelineCreateShaderModule](#shpipelinecreateshadermodule)
    * [shPipelineCreateShaderStage](#shpipelinecreateshaderstage)
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
    * [shGetDescriptorSize](#shgetdescriptorsize)
* Defined at [`shVkDrawLoop.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkDrawLoop.h)
    * [shFrameReset](#shframereset)
    * [shFrameBegin](#shframebegin)
    * [shDrawIndexed](#shdrawindexed)
    * [shDraw](#shdraw)
    * [shFrameEnd](#shframeend)

<button class="btn">[top](#shvulkan-c-definitions)</button>

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

<button class="btn">[top](#shvulkan-c-definitions)</button>

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

<button class="btn">[top](#shvulkan-c-definitions)</button>

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

<button class="btn">[top](#shvulkan-c-definitions)</button>

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

<button class="btn">[top](#shvulkan-c-definitions)</button>

---


## ShVkImageType
```c
typedef enum ShVkImageType {
	SH_SWAPCHAIN_IMAGE = 0b001,
	SH_DEPTH_IMAGE = 0b010
} ShVkImageType;
```

### Description
Enum type required to define the usage of a specific [`VkImage`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImage.html).

<button class="btn">[top](#shvulkan-c-definitions)</button>

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

<button class="btn">[top](#shvulkan-c-definitions)</button>

---

## ShVkFixedStateFlags
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
Some setup flags required when creating a graphics pipeline (see [`shVkSetupGraphicsPipeline`](#shvksetupgraphicspipeline)).

<button class="btn">[top](#shvulkan-c-definitions)</button>

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

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



# Functions and macros



## shCheckValidationLayers
```c
extern uint8_t shCheckValidationLayers(const char* validation_layer);
```

### Description
Loops through the installed validation layers: returns `1` if the given validation layer was found.

### Parameters
 * **`validation_layer`**: valid string naming the required validation layer. 
### Usage example

```c
#include <shvulkan/shVkCheck.h>
#include <stdio.h>

int main(void) {
    if (shCheckValidationLayers("VK_LAYER_KHRONOS_validation")) {
        puts("validation layer found!\n");
    }
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shTranslateVkResult
```c
extern const char* shTranslateVkResult(const VkResult vk_result);
```

### Description
Translates a `VkResult` returned by calling a Vulkan API function. Returns the literal translation of [`vk_result`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html).

### Parameters
 * [**`vk_result`**](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html): the condition.

### Usage example

```c
#include <shvulkan/shVkCheck.h>ì
#include <stdio.h>

int main(void) {
    VkInstance instance = NULL;
    VkInstanceCreateInfo instance_create_info = { 0 };
    VkResult result = vkCreateInstance(&instance_create_info, NULL, &instance);
    //the operation will fail and return an error
    printf("vkCreateInstante result: %s\n", shTranslateVkResult(result));
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shVkError
```c
#define shVkError(condition, error_msg)\
	if ((int)(condition)) {\
		printf("shvulkan error: %s\n", (const char*)(error_msg));\
		exit(-1);\
	}
```

### Description
Prints an error message on the terminal and quits if the condition is not satisfied (bigger or equal to 1).

### Parameters
 * **`condition`**: a condition input, automatically casted to a signed integer `int`;
 * **`error_msg`**: the message (encoded as a `const char*`) to display on the console, when `condition` bigger or equal to 1.  
### Usage example

```c
#include <shvulkan/shVkCheck.h>ì
#include <stdio.h>

int main(void) {
    char* ptr = NULL;
    shVkError(ptr == NULL, "invalid pointer");
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shVkResultError
```c
#define shVkResultError(result, error_msg)\
	if ((VkResult)(result) != VK_SUCCESS) {\
		printf("shvulkan error: %s, %s\n", error_msg, shTranslateVkResult((VkResult)(result)));\
		exit(-1);\
	}
```

### Description
Asserts a [`VkResult`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html), prints an error message if `result` is not equal to `VK_SUCCESS` and quits.

### Parameters
 * **`result`**: [`VkResult`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html) value to check;
 * [**`error_msg`**]: the message (encoded as a `const char*`) to display on the console when the `condition` is lower or equal to zero. 
### Usage example

```c
#include <shvulkan/shVkCheck.h>ì

int main(void) {
    VkInstance instance = NULL;
    VkInstanceCreateInfo instance_create_info = { 0 };
    shVkResultError(
        vkCreateInstance(&instance_create_info, NULL, &instance),
        "invalid instance create info structure"
    );
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateInstance
```c
extern void shCreateInstance(ShVkCore* p_core, const char* application_name, const char* engine_name, const uint8_t enable_validation_layers, const uint32_t extension_count, const char** extension_names);
```

### Description
Initializes a [`VkInstance`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkInstance.html) stored in a [`ShVkCore`](#shvkcore) structure.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`application_name`**: valid application name string;
 * **`engine_name`**: valid engine name string;
 * **`enable_validation_layers`**: if bigger or equal to `1`, enables the [`VK_LAYER_KHRONOS_validation`](https://vulkan.lunarg.com/doc/view/1.2.148.1/windows/khronos_validation_layer.html) layer, useful for debugging;
 * **`extension_count`**: number of instance extensions;
 * **`extension_names`**: array of strings with length equal to the `extension_count` parameter. You might need to enable `VK_KHR_surface` and other surface specific extensions when you want to display the framebuffers images on a window.

### Usage example

```c
#include <shvulkan/shVkCheck.h>
#include <shvulkan/shVkCore.h>ì

int main(void) {

    ShVkCore core = { 0 };

	const char* extension_names[2] = {
        "VK_KHR_surface", 
        "VK_KHR_win32_surface" 
    };//platform dependent: APIs such as glfw automatically detect the required instance extensions

	printf("required instance extensions:\n");
	for (uint32_t i = 0; i < extension_count; i++) {
		printf("%s\n", extension_names[i]);
	}

    shVkAssertResult(
    	shCreateInstance(&core, "my application", "shvulkan engine", 1, 2, extension_names),
        "error creating vulkan instance"
    );

	// [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSelectPhysicalDevice
```c
extern void shSelectPhysicalDevice(ShVkCore* p_core, const VkQueueFlags requirements);
```

### Description
Picks a physical device given a valid [`ShVkCore`](#shvkcore) structure and some requirement flags.

### Parameters
 * **`p_core`**: the instance must have been successfully created with [`shCreateInstance`](#shcreateinstance);
 * **`requirements`**: flags to filter the GPUs which support graphics `SH_VK_CORE_GRAPHICS` or compute operations `SH_VK_CORE_COMPUTE`;
### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	shSelectPhysicalDevice(&core, SH_VK_CORE_GRAPHICS | SH_VK_CORE_COMPUTE);
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetQueueInfo
```c
extern void shSetQueueInfo(const uint32_t queue_family_index, const float* priority, VkDeviceQueueCreateInfo* p_queue_info);
```

### Description
Initializes a [`VkDeviceQueueCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceQueueCreateInfo.html) structure given the queue family index and a priority.

### Parameters
 * **`queue_family_index`**: a queue family index, already set up when selecting the physical device with [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`priority`**: valid pointer to a priority floating point number, generally set to `1.0f`;
 * **`p_queue_info`**: valid pointer to a [`VkDeviceQueueCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceQueueCreateInfo.html) structure.
<button class="btn">[top](#shvulkan-c-definitions)</button>

---


## shSetLogicalDevice
```c
extern void shSetLogicalDevice(ShVkCore* p_core);
```

### Description
Creates a logical device ([`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html)). 

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    shSetLogicalDevice(&core);
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateSwapchain
```c
extern void shCreateSwapchain(ShVkCore* p_core);
```

### Description
Sets up the handle responsible for coordinating the images generated after a rendering operation. Requires a valid [`VkSurfaceKHR`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkSurfaceKHR.html) inside the [`ShVkCore`](#shvkcore) structure.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    shCreateSwapchain(&core);
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shGetSwapchainImages
```c
extern void shGetSwapchainImages(ShVkCore* p_core);
```

### Description
Writes the swapchain images given a valid swapchain, stored at p_core.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    //create surface --> platform dependent
    //setup swapchain
    shGetSwapchainImages(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateSwapchainImageViews
```c
extern void shCreateSwapchainImageViews(ShVkCore* p_core);
```

### Description
Sets up a swapchain [`VkImageView`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImageView.html) handle. Before calling this function you must have initialized the swapchain images ([shGetSwapchainImages](#shgetswapchainimages)).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //create surface --> platform dependent
    //setup swapchain
    //get swapchain images
    shCreateSwapchainImageViews(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateRenderPass
```c
extern void shCreateRenderPass(ShVkCore* p_core);
```

### Description
Creates a [`VkRenderPass`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkRenderPass.html).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    //setup swapchain
    //get swapchain images
    //get swapchain image views
    shCreateRenderPass(ShVkCore* p_core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetFramebuffers
```c
extern void shSetFramebuffers(ShVkCore* p_core);
```

### Description
Sets up a [`VkFramebuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFramebuffer.html) for each swapchain image.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    //create surface --> platform dependent
    //setup swapchain
    //get swapchain images
    //get swapchain image views
    //setup render pass
    shSetFramebuffers(&core);
    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetSyncObjects
```c
extern void shSetSyncObjects(ShVkCore* p_core);
```

### Description
Sets up a [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html) command buffer and an additional [`VkSemaphore`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkSemaphore.html) for each graphics command buffer.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //create command buffers
    shSetSyncObject(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSwapchainRelease
```c
extern void shSwapchainRelease(ShVkCore* p_core);
```

### Description
Frees memory from the swapchain with the relative image views and framebuffers. 

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    //setup swapchain
    //get swapchain images
    //get swapchain image views
    shSwapchainRelease(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shDepthBufferRelease
```c
extern void shDepthBufferRelease(ShVkCore* p_core);
```

### Description
Destroys a depth image view, a depth image and frees the depth image memory.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    //create depth image
    //create depth image view
    shDepthBufferRelease(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSurfaceRelease
```c
extern void shSurfaceRelease(ShVkCore* p_core);
```

### Description
Destroys the `VkSurfaceKHR`. 

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
    shSurfaceRelease(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCmdRelease
```c
extern void shCmdRelease(ShVkCore* p_core);
```

### Description
Destroys the [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s, [`VkCommandPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandPool.html)s and [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html)s. Releases a [`VkSemaphore`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkSemaphore.html) for each graphics command buffer.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    //create command buffers
    //create sync objects

    shCmdRelease(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shRenderPassRelease
```c
extern void shRenderPassRelease(ShVkCore* p_core);
```

### Description
Destroys the [`VkRenderPass`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkRenderPass.html) stored at `p_core`.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //create surface --> platform dependent
	//setup physical device
    //setup logical device
    //create surface --> platform dependent
    //setup swapchain
    //get swapchain images
    //get swapchain image views
    //setup render pass
    
    //destroy swapchain data
    //destroy surface
    shRenderPassRelease(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shInstanceRelease
```c
extern void shInstanceRelease(ShVkCore* p_core);
```

### Description
Destroys the [`VkInstance`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkInstance.html) stored at `p_core`.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    shDestroyInstance(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shVulkanRelease
```c
extern void shVulkanRelease(ShVkCore* p_core);
```

### Description
Automatically destroys every active Vulkan object stored at `p_core`.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup
    
    shVulkanRelease(&core);
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shGetGraphicsQueue
```c
extern void shGetGraphicsQueue(ShVkCore* p_core);
```

### Description
Gets graphics [`VkQueue`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkQueue.html) handle for submitting rendering data to the GPU.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    shGetGraphicsQueue(&core);
    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shGetComputeQueue
```c
extern void shGetComputeQueue(ShVkCore* p_core);
```

### Description
Gets compute [`VkQueue`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkQueue.html) handle for submitting rendering data to the GPU.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    shGetComputeQueue(&core);
    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shInitSwapchainData
```c
#define shInitSwapchainData(p_core) shCreateSwapchain(p_core); shGetSwapchainImages(p_core); shCreateSwapchainImageViews(p_core)
```

### Description
Macro definition used to call [`shCreateSwapchain`](#shcreateswapchain), [`shGetSwapchainImages`](#shgetswapchainimages) and [`shCreateSwapchainImageViews`](#shcreateswapchainimageviews).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    //create surface --> platform dependent
    shInitSwapchainData(&core);
    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateGraphicsCommandBuffers

```c
#define shCreateGraphicsCommandBuffers(p_core, thread_count)\
	shCreateCommandData(p_core, VK_QUEUE_GRAPHICS_BIT, thread_count, &(p_core)->p_graphics_commands)\
```

### Description
Builds a `thread_count` number of graphics [`VkCommandPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandPool.html)s and [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html)s.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`thread_count`**: number of threads.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    shCreateGraphicsCommandBuffers(&core, 1);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateComputeCommandBuffers

```c
#define shCreateComputeCommandBuffers(p_core, thread_count)\
	shCreateCommandData(p_core, VK_QUEUE_COMPUTE_BIT, thread_count, &(p_core)->p_compute_commands)\
```

### Description
Builds a `thread_count` number of compute [`VkCommandPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandPool.html)s and [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html)s.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`thread_count`**: number of threads.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    shCreateComputeCommandBuffers(&core, 1);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shResetCommandBuffer
```c
#define shResetCommandBuffer(cmd_buffer) vkResetCommandBuffer(cmd_buffer, 0)
```

### Description
Resets a command buffer to its initial state, calls [`vkResetCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkResetCommandBuffer.html).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    uint32_t thread = 0;//same process valid with compute command buffers
    shResetCommandBuffer(core.p_compute_commands[thread].cmd_buffer);//compute

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shResetFences
```c
#define shResetFences(device, fence_count, p_fences) vkResetFences(device, fence_count, p_fences);
```

### Description
Resets a `fence_count` number of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s to their initial state, calls [`vkResetCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkResetCommandBuffer.html).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`fence_count`**: number of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s to reset;
 * **`p_fences`**: valid array of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s with length equal to `fence_count`.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 3;
    //setup command buffers
    //create sync objects

    //reset command buffers

    VkFence fences[3] = {//same process valid with graphics fences
        core.p_compute_commands[0].fence, 
        core.p_compute_commands[1].fence,
        core.p_compute_commands[2].fence
    };
    shResetFences(core.device, thread_count, fences);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shResetFence
```c
#define shResetFence(device, p_fence) vkResetFences(device, 1, p_fence);
```

### Description
Resets a [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html) to its initial state, calls [`vkResetCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkResetCommandBuffer.html).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`p_fence`**: valid pointer to a [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 1;
    //setup command buffers
    //create sync objects

    //reset command buffer

    //same process valid with graphics fences
    shResetFence(core.device, &core.p_compute_commands[0].fence);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBeginCommandBuffer
```c
extern void shBeginCommandBuffer(const VkCommandBuffer cmd_buffer);
```

### Description
Starts recording a [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html).

### Parameters
 * **`cmd_buffer`**: valid [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers).

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 1;
    //setup command buffers
    //create sync objects

    //reset command buffer
    //reset fence

    //same process valid with graphics command buffers
	shBeginCommandBuffer(core.p_compute_commands[0].cmd_buffer);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shQueueSubmit
```c
extern void shQueueSubmit(VkCommandBuffer* cmd_buffer, const VkQueue queue, VkFence fence);
```

### Description
Submits rendering data to the GPU. 

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers).

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 1;
    //setup command buffers
    //create sync objects

    //same process valid with graphics command buffers and queues
    
    //reset command buffer
    //reset fence
    //begin command buffer

    //[...]

    //end command buffer
    shQueueSubmit(&core.p_compute_commands[0].cmd_buffer, core.compute_queue.queue, core.p_compute_commands[0].fence);


    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCmdDispatch
```c
#define shCmdDispatch(cmd_buffer, group_count_x, group_count_y, group_count_z) vkCmdDispatch(cmd_buffer, group_count_x, group_count_y, group_count_z)
```

### Description
Dispatches compute work groups along x, y, and z dimensions. 

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`group_count_x`**: number of work groups at dimension x;
 * **`group_count_y`**: number of work groups at dimension y;
 * **`group_count_z`**: number of work groups at dimension z;
### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 1;
    //setup command buffers
    //create sync objects

    //reset command buffer
    //reset fence
    //begin command buffer

    //[...]

    shCmdDispatch(core.p_compute_commands[0].cmd_buffer, 8, 8, 1);

    //end command buffer
    //submit queue

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shWaitForFences
```c
#define shWaitForFences(device, fence_count, p_fences) vkWaitForFences(device, fence_count, p_fences, VK_TRUE, 100000000000)
```

### Description
Waits for a `fence_count` number of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s to unlock.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`fence_count`**: number of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s to wait for;
 * **`p_fences`**: pointer to an array of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s with length equal to `fence_count`, see [`shSetSyncObjects`](#shsetsyncobjects);
### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 3;
    //setup command buffers
    //create sync objects

    //reset command buffers
    //reset fences
    //begin command buffers

    //[...]

    //end command buffers
    //submit queue

    //same process valid with graphics command buffers and fences

    VkFence fences[3] = {
        core.p_compute_commands[0].fence,
        core.p_compute_commands[1].fence,
        core.p_compute_commands[2].fence
    };
    shWaitForFences(core.device, thread_count, fences);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shWaitForFence
```c
#define shWaitForFence(device, p_fence) vkWaitForFences(device, 1, p_fence, VK_TRUE, 100000000000)
```

### Description
Waits for a [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html) to unlock.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`p_fences`**: pointer to a valid [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html), see [`shSetSyncObjects`](#shsetsyncobjects);
### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 1;
    //setup command buffers
    //create sync objects

    //reset command buffers
    //reset fences
    //begin command buffers

    //[...]

    //end command buffers
    //submit queue

    //same process valid with graphics command buffers and fences

    shWaitForFence(core.device, &core.compute_commands[0].fence);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shEndCommandBuffer
```c
#define shEndCommandBuffer(cmd_buffer) vkEndCommandBuffer(cmd_buffer)
```

### Description
Ends a [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), stops the command buffer recording state.

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers), [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [shBeginCommandBuffer](#shbegincommandbuffer).

### Usage example

```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    uint32_t thread_count = 1;
    //setup command buffers
    //create sync objects

    //same process valid with graphics command buffers

    //reset command buffers
    //reset fences
    //begin command buffers

    //[...]

    shEndCommandBuffer(core.p_compute_commands[0].cmd_buffer);
    //submit queue

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateBuffer
```c
extern void shCreateBuffer(const VkDevice device, const uint32_t size, VkBufferUsageFlags usage_flags, VkBuffer* p_buffer);
```

### Description
Creates a Vulkan buffer object known as [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`size`**: size in bytes of the buffer; 
 * **`usage_flags`**: [`VkBufferUsageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBufferUsageFlags.html) enum type representing what the Vulkan buffer is going to be used for, see [`VkBufferUsageFlagBits`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBufferUsageFlagBits.html); 
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer buffer;
    shCreateBuffer(core.device, 20, VK_BUFFER_USAGE_STORAGE_BUFFER_BIT, &buffer);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shGetMemoryType
```c
extern void shGetMemoryType(const VkDevice device, const VkPhysicalDevice physical_device, const VkMemoryPropertyFlags property_flags, uint32_t *p_memory_type_index);
```

### Description
Gets the most suitable memory type index before allocating memory.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice); 
 * **`property_flags`**: [`VkMemoryPropertyFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkMemoryPropertyFlags.html) enum type representing specific properties of the buffer memory, see [`VkBufferUsageFlagBits`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkMemoryPropertyFlagBits.html);
 * **`p_memory_type_index`**: valid pointer to an unsigned integer which is going to carry the memory type index. 
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    uint32_t memory_type_index = 0;
    VkMemoryPropertyFlags property_flags = VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT | VK_MEMORY_PROPERTY_HOST_COHERENT_BIT;
	shGetMemoryType(core.device, core.physical_device, property_flags, &memory_type_index);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shAllocateMemory
```c
extern void shAllocateMemory(const VkDevice device, const VkPhysicalDevice physical_device, const VkBuffer buffer, const VkMemoryPropertyFlags property_flags, VkDeviceMemory* p_memory);
```

### Description
Gets the most suitable memory type index and allocates memory on the GPU.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice); 
 * **`buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html), see [`shCreateBuffer`](#shcreatebuffer);
 * **`property_flags`**: [`VkMemoryPropertyFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkMemoryPropertyFlags.html) enum type representing specific properties of the buffer memory, see [`VkBufferUsageFlagBits`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkMemoryPropertyFlagBits.html);
 * **`p_memory`**: valid pointer to a [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle. 
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer buffer;
    //create buffer

    VkDeviceMemory buffer_memory;
    VkMemoryPropertyFlags property_flags = VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT | VK_MEMORY_PROPERTY_HOST_COHERENT_BIT;
    shAllocateMemory(core.device, core.physical_device, buffer, property_flags, &buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBindMemory
```c
#define shBindMemory(device, vk_buffer, memory)\
	shVkAssertResult(\
		vkBindBufferMemory(device, vk_buffer, memory, 0),\
		"error binding buffer memory "\
	)
```

### Description
Binds a specific [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice); 
 * **`vk_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html), see [`shCreateBuffer`](#shcreatebuffer);
 * **`memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle, see [`shAllocateMemory`](#shallocatememory).

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer buffer;
    //create buffer

    VkDeviceMemory buffer_memory;
    //allocate memory

    // [...]

    shBindMemory(core.device, buffer, buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shReadMemory
```c
extern void shReadMemory(const VkDevice device, const VkDeviceMemory memory, const uint32_t offset, const uint32_t data_size, void* p_data);
```

### Description
Reads data from a [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle and writes it all at `p_data` block.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle, see [`shAllocateMemory`](#shallocatememory);
 * **`offset`**: the source device memory data offset in bytes;
 * **`data_size`**: size in bytes of the data to read;
 * **`p_data`**: pointer to the destination buffer with size at least equal to `data_size`;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    //create buffer

    VkDeviceMemory buffer_memory;
    //allocate memory

    // [...]

    float output[16];
    shReadMemory(core.device, buffer_memory, 0, sizeof(output), output);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shWriteMemory
```c
extern void shWriteMemory(const VkDevice device, const VkDeviceMemory memory, const uint32_t offset, const uint32_t data_size, const void* p_data);
```

### Description
Writes data on the GPU, according to the specified [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle, see [`shAllocateMemory`](#shallocatememory);
 * **`offset`**: the destination device memory data offset in bytes;
 * **`data_size`**: size in bytes of the data to write;
 * **`p_data`**: pointer to the source buffer with size at least equal to `data_size`;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    //create buffer

    VkDeviceMemory buffer_memory;
    //allocate memory

    // [...]

    float src[16] = {
        1.0f, 1.0f, 2.0f, 0.0f,
        0.0f, 4.0f, 0.0f, 0.0f,
        0.5f, 0.0f, 5.0f, 0.0f,
        0.0f, 0.0f, 2.0f, 1.0f
    };
    shWriteMemory(core.device, buffer_memory, 0, sizeof(src), src);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shClearBufferMemory
```c
extern void shClearBufferMemory(const VkDevice device, const VkBuffer buffer, const VkDeviceMemory memory);
```

### Description
Destroys a [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) and clears the relative device memory.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) handle, see [`shCreateBuffer`](#shcreatebuffer);
 * **`memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle, see [`shAllocateMemory`](#shallocatememory);
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer buffer;
    //create buffer

    VkDeviceMemory buffer_memory;
    //allocate memory

    // [...]

    shClearBufferMemory(core.device, buffer, buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---




## shCreateImage
```c
extern void shCreateImage(const VkDevice device, const VkPhysicalDevice physical_device, const uint32_t width, const uint32_t height, VkFormat format, VkImageUsageFlags usage, VkImage* p_image, VkDeviceMemory* p_image_memory);
```

### Description
Creates a Vulkan image handle and allocates the required image memory.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid [`VkPhysicalDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDevice.html) handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`width`**: width of the image in pixels;
 * **`height`**: height of the image in pixels;
 * **`format`**: [`VkFormat`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFormat.html) enum value, if you want to present the image remember to check the supported formats with [`vkGetPhysicalDeviceSurfaceFormatsKHR`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkGetPhysicalDeviceSurfaceFormatsKHR.html), (`VK_KHR_surface` would be required);
 * **`usage`**: [`VkImageUsageFlagBits`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImageUsageFlagBits.html) enum value;
 * **`p_image`**: valid pointer to a [`VkImage`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImage.html) object;
 * **`p_image_memory`**: valid pointer to a [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImage.html) handle;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device

    VkImage image;
    VkImageMemory image_memory;

    shCreateImage(core.device, core.physical_device, 720, 480, VK_FORMAT_R8G8B8A8_UNORM, VK_IMAGE_USAGE_COLOR_ATTACHMENT_BIT, &image, &image_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shGetMemoryBudgetProperties
```c
extern void shGetMemoryBudgetProperties(const VkPhysicalDevice physical_device, uint32_t* p_memory_budget, uint32_t* p_process_used_memory, VkPhysicalDeviceMemoryBudgetPropertiesEXT* p_memory_budget_properties);
```

### Description
Gets the amount of VRAM ready for use and the memory used by other processes. To work it requires [`VkPhysicalDeviceMemoryBudgetPropertiesEXT`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDeviceMemoryBudgetPropertiesEXT.html) (already activated when creating the logical device with [shSetLogicalDevice](#shsetlogicaldevice) if supported by the user machine).

### Parameters
 * **`physical_device`**: valid [`VkPhysicalDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDevice.html) handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`p_memory_budget`**: optional pointer to an unsigned integer, displays in bytes the unused VRAM;
 * **`p_process_used_memory`**: optional pointer to an unsigned integer, displays in bytes the used VRAM by the current process;
 * **p_memory_budget_properties**: optional pointer to a [`VkPhysicalDeviceMemoryBudgetPropertiesEXT`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDeviceMemoryBudgetPropertiesEXT.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device

    uint32_t availble_vram = 0;
    uint32_t used_vram = 0;
    shGetMemoryBudgetProperties(core.physical_device, &available_vram, &used_vram, NULL);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateVertexBuffer
```c
#define shCreateVertexBuffer(device, size, p_vertex_buffer)\
	shCreateBuffer(device, size, VK_BUFFER_USAGE_VERTEX_BUFFER_BIT, p_vertex_buffer)
```

### Description
Creates a vertex buffer. Calls [`shCreateBuffer`](#shcreatebuffer).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`size`**: size in bytes of the buffer;
 * **`p_vertex_buffer`**: valid pointer to a [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    float vertices[9] = {
		-1.0f, 1.0f, 0.0f,
		 0.0f, 0.0f, 0.0f,
		 1.0f, 1.0f, 0.0f
    };

    VkBuffer vertex_buffer;
    shCreateVertexBuffer(core.device, sizeof(vertices), &vertex_buffer);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shAllocateVertexBufferMemory
```c
#define shAllocateVertexBufferMemory(device, physical_device, vertex_buffer, p_vertex_buffer_memory)\
	shAllocateMemory(device, physical_device, vertex_buffer, VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT | VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_DEVICE_LOCAL_BIT, p_vertex_buffer_memory)
```

### Description
Allocates the vertex buffer memory. Calls [`shAllocateMemory`](#shallocatememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid [`VkPhysicalDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDevice.html) physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`vertex_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object;
 * **`p_vertex_buffer_memory`**: valid pointer to a [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer vertex_buffer;
    //create vertex buffer

    VkDeviceMemory vertex_buffer_memory;
    shAllocateVertexBufferMemory(core.device, core.physical_device, vertex_buffer, &vertex_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBindVertexBufferMemory
```c
#define shBindVertexBufferMemory(device, vertex_buffer, vertex_buffer_memory)\
	shBindMemory(device, vertex_buffer, vertex_buffer_memory)
```

### Description
Binds a specific vertex [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle. Calls [`shBindMemory`](#shbindmemory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`vertex_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object;
 * **`vertex_buffer_memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer vertex_buffer;
    //create vertex buffer

    VkDeviceMemory vertex_buffer_memory;
    //allocate vertex buffer memory

    shBindVertexBufferMemory(core.device, vertex_buffer, vertex_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shWriteVertexBufferMemory
```c
#define shWriteVertexBufferMemory(device, vertex_buffer_memory, size, p_vertices)\
	shWriteMemory(device, vertex_buffer_memory, 0, size, (void*)p_vertices)
```

### Description
Writes vertex buffer data. Calls [`shWriteMemory`](#shwritememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`vertex_buffer_memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle;
 * **`size`**: size in bytes of the data to write;
 * **`p_vertices`**: pointer to the source buffer with size at least equal to `size`;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    //create vertex buffer

    VkDeviceMemory vertex_buffer_memory;
    //allocate vertex buffer memory

    float vertices[9] = {
		-1.0f, 1.0f, 0.0f,
		 0.0f, 0.0f, 0.0f,
		 1.0f, 1.0f, 0.0f
    };

    shWriteVertexBufferMemory(core.device, vertex_buffer_memory, sizeof(vertices), vertices);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBindVertexBuffer
```c
static void shBindVertexBuffer(VkCommandBuffer graphics_cmd_buffer, VkBuffer* p_vertex_buffer) {
	const VkDeviceSize offset = 0;
	vkCmdBindVertexBuffers(graphics_cmd_buffer, 0, 1, p_vertex_buffer, &offset);
}
```

### Description
Binds the index buffer with a command buffer. The command buffer must be recording, see [`shBeginCommandBuffer`](#shbegincommandbuffer).

### Parameters
 * **`graphics_cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`p_vertex_buffer`**: valid pointer to a vertex [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    //create vertex buffer

    VkDeviceMemory vertex_buffer_memory;
    //allocate vertex buffer memory

    //begin command buffer
    
    uint32_t thread = 0;
    shBindVertexBuffer(core.p_graphics_commands[thread].cmd_buffer, &vertex_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateIndexBuffer
```c
#define shCreateIndexBuffer(device, size, p_index_buffer)\
	shCreateBuffer(device, size, VK_BUFFER_USAGE_INDEX_BUFFER_BIT, p_index_buffer)
```

### Description
Creates an index buffer. Calls [`shCreateBuffer`](#shcreatebuffer).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`size`**: size in bytes of the buffer;
 * **`p_index_buffer`**: valid pointer to a [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    uint32_t indices[3] = {
		0, 1, 2
    };

    VkBuffer index_buffer;
    shCreateIndexBuffer(core.device, sizeof(indices), &index_buffer);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shAllocateIndexBufferMemory
```c
#define shAllocateIndexBufferMemory(device, physical_device, index_buffer, p_index_buffer_memory)\
	shAllocateMemory(device, physical_device, index_buffer, VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT | VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_DEVICE_LOCAL_BIT, p_index_buffer_memory)
```

### Description
Allocates index buffer memory. Calls [`shAllocateMemory`](#shallocatememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid [`VkPhysicalDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDevice.html) physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`index_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object;
 * **`p_index_buffer_memory`**: valid pointer to a [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer index_buffer;
    //create index buffer

    VkDeviceMemory index_buffer_memory;
    shAllocateIndexBufferMemory(core.device, core.physical_device, index_buffer, &index_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBindIndexBufferMemory
```c
#define shBindIndexBufferMemory(device, index_buffer, index_buffer_memory)\
	shBindMemory(device, index_buffer, index_buffer_memory)
```

### Description
Binds a specific index [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle. Calls [`shBindMemory`](#shbindmemory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`vertex_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object;
 * **`vertex_buffer_memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer index_buffer;
    //create index buffer

    VkDeviceMemory index_buffer;
    //allocate index buffer memory

    shBindIndexBufferMemory(core.device, index_buffer, index_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shWriteIndexBufferMemory
```c
#define shWriteIndexBufferMemory(device, index_buffer_memory, size, p_indices)\
	shWriteMemory(device, index_buffer_memory, 0, size, (void*)p_indices)
```

### Description
Writes index buffer data. Calls [`shWriteMemory`](#shwritememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`index_buffer_memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle;
 * **`size`**: size in bytes of the data to write;
 * **`p_indices`**: pointer to the source buffer with size at least equal to `size`;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    //create index buffer

    VkDeviceMemory index_buffer_memory;
    //allocate index buffer memory

    uint32_t indices[3] = {
		0, 1, 2
    };

    shWriteIndexBufferMemory(core.device, index_buffer_memory, sizeof(indices), indices);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBindIndexBuffer
```c
#define shBindIndexBuffer(graphics_cmd_buffer, p_index_buffer)\
	vkCmdBindIndexBuffer(graphics_cmd_buffer, *p_index_buffer, 0, VK_INDEX_TYPE_UINT32)
```

### Description
Binds the index buffer with a command buffer. The command buffer must be recording, see [`shBeginCommandBuffer`](#shbegincommandbuffer).

### Parameters
 * **`graphics_cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`p_index_buffer`**: valid pointer to an index [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) object;
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    //create index buffer

    VkDeviceMemory index_buffer_memory;
    //allocate index buffer memory

    //begin command buffer
    
    uint32_t thread = 0;
    shBindIndexBuffer(core.p_graphics_commands[thread].cmd_buffer, &index_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shClearVertexBufferMemory
```c
#define shClearVertexBufferMemory(device, vertex_buffer, vertex_buffer_memory)\
	shClearBufferMemory(device, vertex_buffer, vertex_buffer_memory)
```

### Description
Destroys a vertex [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) and clears the relative device memory. Call [`shClearBufferMemory`](#shclearbuffermemory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`vertex_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) handle, see [`shCreateBuffer`](#shcreatebuffer);
 * **`vertex_buffer_memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle, see [`shAllocateMemory`](#shallocatememory);
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer vertex_buffer;
    //create vertex buffer

    VkDeviceMemory vertex_buffer_memory;
    //allocate vertex buffer memory

    shClearVertexBufferMemory(core.device, vertex_buffer, vertex_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shClearIndexBufferMemory
```c
#define shClearIndexBufferMemory(device, index_buffer, index_buffer_memory)\
	shClearBufferMemory(device, index_buffer, index_buffer_memory)
```

### Description
Destroys an index [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) and clears the relative device memory. Call [`shClearBufferMemory`](#shclearbuffermemory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`index_buffer`**: valid [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) handle, see [`shCreateBuffer`](#shcreatebuffer);
 * **`index_buffer_memory`**: valid [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle, see [`shAllocateMemory`](#shallocatememory);
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    VkBuffer index_buffer;
    //create index buffer

    VkDeviceMemory index_buffer_memory;
    //allocate index buffer memory

    shClearIndexBufferMemory(core.device, index_buffer, index_buffer_memory);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineAllocateDescriptorBufferMemory
```c
#define shPipelineAllocateDescriptorBufferMemory(device, physical_device, descriptor_idx, p_pipeline)\
	shAllocateMemory(device, physical_device, (p_pipeline)->descriptor_buffers[descriptor_idx], VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT | VK_MEMORY_PROPERTY_HOST_COHERENT_BIT | VK_MEMORY_PROPERTY_DEVICE_LOCAL_BIT, &(p_pipeline)->descriptor_buffers_memory[descriptor_idx])
```

### Description
Allocates descriptor buffer memory. Calls [`shAllocateMemory`](#shallocatememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid [`VkPhysicalDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPhysicalDevice.html) physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    ShVkPipeline pipeline = { 0 };

    //create descriptor buffer

    uint32_t descriptor_idx = 0;
    shPipelineAllocateDescriptorBufferMemory(core.device, core.physical_device, descriptor_idx, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineBindDescriptorBufferMemory
```c
#define shPipelineBindDescriptorBufferMemory(device, descriptor_idx, p_pipeline)\
	shBindMemory(device, (p_pipeline)->descriptor_buffers[descriptor_idx], (p_pipeline)->descriptor_buffers_memory[descriptor_idx])
```

### Description
Binds a specific descriptor [`VkDeviceMemory`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceMemory.html) handle. Calls [`shBindMemory`](#shbindmemory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    ShVkPipeline pipeline = { 0 };

    //create descriptor buffer
    //allocate descriptor buffer memory

    // [...]

    uint32_t descriptor_idx = 0;
    shPipelineBindDescriptorBufferMemory(core.device, descriptor_idx, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineClearDescriptorBufferMemory
```c
#define shPipelineClearDescriptorBufferMemory(device, descriptor_idx, p_pipeline)\
	shClearBufferMemory(device, (p_pipeline)->descriptor_buffers[descriptor_idx], (p_pipeline)->descriptor_buffers_memory[descriptor_idx])
```

### Description
Destroys a descriptor [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) and clears the relative device memory. Call [`shClearBufferMemory`](#shclearbuffermemory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    ShVkPipeline pipeline = { 0 };

    //create descriptor buffer
    //allocate descriptor buffer memory

    uint32_t descriptor_idx = 0;
    shPipelineClearDescriptorBufferMemory(core.device, descriptor_idx, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateDepthImage
```c
#define shCreateDepthImage(p_core)\
	shCreateImage((p_core)->device, (p_core)->physical_device, (p_core)->surface.width, (p_core)->surface.height, SH_DEPTH_IMAGE_FORMAT, VK_IMAGE_USAGE_DEPTH_STENCIL_ATTACHMENT_BIT, &(p_core)->depth_image, &(p_core)->depth_image_memory)
```

### Description
Creates a depth image. Requires a valid [`VkSurfaceKHR`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkSurfaceKHR.html) inside the [`ShVkCore`](#shvkcore) structure.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    shCreateDepthImage(&core);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateDepthImageView
```c
#define shCreateDepthImageView(p_core) shCreateImageView(p_core, (p_core)->depth_image, SH_DEPTH_IMAGE, &(p_core)->depth_image_view)
```

### Description
Macro definition for creating a depth [`VkImageView`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImageView.html).

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    //create surface --> platform dependent
    //create depth image
    shCreateDepthImageView(&core);
    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shInitDepthData
```c
#define shInitDepthData(p_core)\
	shCreateDepthImage(p_core); shCreateDepthImageView(p_core)
```

### Description
Creates a depth image and a depth image view object. Calls [`shCreateDepthImage`](#shcreatedepthimage) and [`shCreateDepthImageView`](#shcreatedepthimageview)

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    //create surface --> platform dependent
    
    shInitDepthData(&core);
    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateRasterizer
```c
extern void shCreateRasterizer(VkPipelineRasterizationStateCreateInfo* p_rasterizer);
```

### Description
Creates a rasterizer handle to draw pixel on the framebuffer.

### Parameters
 * **`p_rasterize`**: valid pointer to a [`VkPipelineRasterizationStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineRasterizationStateCreateInfo.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkPipeline graphics_pipeline = { 0 };
    shCreateRasterizer(&graphics_pipeline.rasterizer);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetMultisampleState
```c
extern void shSetMultisampleState(VkPipelineMultisampleStateCreateInfo* p_multisample_state);
```

### Description
Sets multisample infos.

### Parameters
 * **`p_multisample_state`**: valid pointer to a [`VkPipelineMultisampleStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineMultisampleStateCreateInfo.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkPipeline graphics_pipeline = { 0 };
    shSetMultisampleState(&graphics_pipeline.multisample_state_info);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shColorBlendSettings
```c
extern void shColorBlendSettings(VkPipelineColorBlendAttachmentState* p_color_blend_attachment, VkPipelineColorBlendStateCreateInfo* p_color_blend_state);
```

### Description
Sets up some color blending properties.

### Parameters
 * **`p_color_blend_attachment`**: valid pointer to a [`VkPipelineColorBlendAttachmentState`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineColorBlendAttachmentState.html) structure;
 * **`p_color_blend_state`**: valid pointer to a [`VkPipelineColorBlendStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineColorBlendStateCreateInfo.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkFixedStates fixed_states = { 0 };
   	shColorBlendSettings(&fixed_states.color_blend_attachment, &p_fixed_states.color_blend_state);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetViewport
```c
extern void shSetViewport(const uint32_t width, const uint32_t height, VkViewport *p_viewport, VkRect2D* p_scissors, VkPipelineViewportStateCreateInfo* p_viewport_state);
```

### Description
Fills some viewport related structures.

### Parameters
 * **`width`**: width in pixels of the viewport;
 * **`height`**: height in pixels of the viewport;
 * **`p_viewport`**: valid pointer to a [`VkViewport`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkViewport.html) structure;
 * **`p_scissors`**: valid pointer to a [`VkRect2D`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkRect2D.html) structure;
 * **`p_viewport_state`**: valid pointer to a [`VkPipelineColorBlendStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineViewportStateCreateInfo.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    uint32_t surface_width  = 720;
    uint32_t surface_height = 480;

    ShVkFixedStates fixed_states = { 0 };
   	shSetViewport(surface_width, surface_height, &fixed_states.viewport, &fixed_states.scissor, &fixed_states.viewport_state);

    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetFixedStates
```c
extern void shSetFixedStates(VkDevice device, const uint32_t surface_width, const uint32_t surface_height, ShVkFixedStateFlags  flags, ShVkFixedStates* p_fixed_states);
```

### Description
Sets up the [`ShVkFixedStates`](#shvkfixedstates) structure.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`surface_width`**: width in pixels of the viewport;
 * **`surface_height`**: height in pixels of the viewport;
 * **`flags`**: [`ShVkFixedStateFlags`](#shvkfixedstateflags) enum value, specifies the polygon mode and the primitive topology, and it visually affects the result of a draw call;
 * **`p_fixed_states`**: valid pointer to a [`ShVkFixedStates`](#shvkfixedstates) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    //you may want to setup a surface and make the viewport dimensions coherent with the window size
    uint32_t surface_width  = 720;
    uint32_t surface_height = 480;

    ShVkFixedStates fixed_states = { 0 };

    // [...]

   	shSetFixedStates(core.device, surface_width, surface_height, SH_FIXED_STATES_POLYGON_MODE_FACE | SH_FIXED_STATES_PRIMITIVE_TOPOLOGY_TRIANGLE_LIST, &fixed_states);

    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetVertexInputAttribute
```c
extern void shSetVertexInputAttribute(const uint32_t location, VkFormat format, const uint32_t offset, const uint32_t size, ShVkFixedStates* p_fixed_states);
```

### Description
Creates a shader vertex buffer input attributes.

### Parameters
 * **`location`**: vertex input shader location;
 * **`format`**: depends on the size and on the input type;
 * **`offset`**: vertex input stride in bytes;
 * **`size`**: size in bytes of the vertex input buffer;
 * **`p_fixed_states`**: valid pointer to a [`ShVkFixedStates`](#shvkfixedstates) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkFixedStates fixed_states = { 0 };
    
    shSetVertexInputAttribute(0, SH_VEC3_SIGNED_FLOAT, 0, 12 &fixed_states);
	shSetVertexInputAttribute(1, SH_VEC3_SIGNED_FLOAT, 12, 12, &fixed_states);
	shSetVertexInputAttribute(2, SH_VEC2_SIGNED_FLOAT, 24, 8, &fixed_states);

    
    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460
layout (location = 0) in vec3 position;
layout (location = 1) in vec3 normal;
layout (location = 2) in vec2 uv;

//shader.vert
// [...]
```
<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetVertexInputState
```c
extern void shSetVertexInputState(VkVertexInputBindingDescription* p_vertex_binding, uint32_t vertex_input_attribute_count, VkVertexInputAttributeDescription* p_vertex_input_attributes, VkPipelineVertexInputStateCreateInfo* p_vertex_input_state);
```

### Description
Builds a [`VkPipelineVertexInputStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineVertexInputStateCreateInfo.html) structure after defining all the vertex input attributes.

### Parameters
 * **`p_vertex_binding`**: valid pointer to a [`VkVertexInputBindingDescription`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkVertexInputBindingDescription.html) structure;
 * **`vertex_input_attribute_count`**: number of vertex input attributes;
 * **`p_vertex_input_attributes`**: pointer to a buffer of [`VkVertexInputAttributeDescription`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkVertexInputAttributeDescription.html) with length at least equal to `vertex_input_attribute_count`;
 * **`p_vertex_input_state`**: valid pointer to a [`VkPipelineVertexInputStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineVertexInputStateCreateInfo.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkFixedStates fixed_states = { 0 };
    
    //set vertex input attributes
    
    shSetVertexInputState(&fixed_states.vertex_binding_description, fixed_states.vertex_input_attribute_description_count, fixed_states.vertex_input_attributes, fixed_states.vertex_input_state_info);

    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateInputAssembly
```c
extern void shCreateInputAssembly(const VkPrimitiveTopology primitive_topology, const VkBool32 primitive_restart_enable, VkPipelineInputAssemblyStateCreateInfo* p_input_assembly);
```

### Description
Creates a [`VkPipelineInputAssemblyStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineInputAssemblyStateCreateInfo.html) structure given the necessary parameters.

### Parameters
 * **`primitive_topology`**: [`VkPrimitiveTopology`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPrimitiveTopology.html) enum value which specifies the primitive topology;
 * **`primitive_restart_enable`**: ;
 * **`p_vertex_input_attributes`**: pointer to a buffer of [`VkVertexInputAttributeDescription`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkVertexInputAttributeDescription.html) with length at least equal to `vertex_input_attribute_count`;
 * **`p_input_assembly`**: valid pointer to a [`VkPipelineInputAssemblyStateCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineInputAssemblyStateCreateInfo.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkFixedStates fixed_states = { 0 };
    
    //setup vertex input attributes
    //setup vertex input state

   	shCreateInputAssembly(VK_PRIMITIVE_TOPOLOGY_TRIANGLE_LIST, VK_FALSE, &fixed_states.input_assembly);

    
    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetPushConstants
```c
extern void shSetPushConstants(const VkShaderStageFlags shader_stage_flags, const uint32_t offset, const uint32_t size, ShVkPipeline* p_pipeline);
```

### Description
Sets up a [`VkPushConstantRange`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPushConstantRange.html) structure, which represents a Vulkan specific type of shader inputs. 

### Parameters
 * **`shader_stage_flags`**: the shader stage where the push costant is going to be specified;
 * **`offset`**: offset in bytes for future bindings;
 * **`size`**: size in bytes of the push constant data;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    VkPushConstantRange push_constant_range = { 0 };

    shSetPushConstants(VK_SHADER_STAGE_VERTEX_BIT, 0, 128, &push_constant_range);
    
    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

//max size: 128 bytes
layout (push_constant) uniform pushConstant {
    mat4 projection;
    mat4 view;
} pconst;

//shader.vert
// [...]
```<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateDescriptorBuffer
```c
extern void shCreateDescriptorBuffer(const VkDevice device, const VkBufferUsageFlags usage, const uint32_t descriptor_idx, const uint32_t size, const uint32_t max_size, VkDescriptorBufferInfo* p_buffer_info, VkBuffer* p_buffer);
```

### Description
Creates a descriptor [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html). 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`usage`**: some common [`VkBufferUsageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBufferUsageFlags.html) values used to create descriptor buffer are `VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT` and `VK_BUFFER_USAGE_STORAGE_BUFFER_BIT`;
 * **`descriptor_idx`**: descriptor set index;
 * **`size`**: size in bytes of the buffer;
 * **`max_size`**: must be equal or a multiple of `size` (generally `max_size` is higher than size when you have to work with dynamic descriptors);
 * **`p_buffer_info`**: valid pointer to a [`VkDescriptorBufferInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorBufferInfo.html) structure, which summarizes the information specified after calling this function.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    VkBuffer descriptor_buffer;
    VkDescriptorBufferInfo descriptor_buffer_info;

    shCreateDescriptorBuffer(
        core.device, 
        VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT, 
        0, 
        64, 
        64, 
        &descriptor_buffer_info, 
        &descriptor_buffer
    );


    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

layout (set = 0, binding = 0) uniform uniformBuffer {
    mat4 model;
} ubo;

// [...]
```<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shDescriptorSetLayout
```c
extern void shDescriptorSetLayout(const VkDevice device, const uint32_t binding, const VkDescriptorType descriptor_type, const VkShaderStageFlags shaderStageFlags, VkDescriptorSetLayoutBinding* p_binding, VkDescriptorSetLayout* p_descriptor_set_layout);
```

### Description
Fills a [`VkDescriptorSetLayoutBinding`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayoutBinding.html) structure and creates a [`VkDescriptorSetLayout`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayout.html) object. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`binding`**:  binding number of the entry and corresponds to a resource of the same binding number in the shader stages, see [`shPipelineBindDescriptorBufferMemory`](#shpipelinebinddescriptorbuffermemory);
 * **`descriptor_type`**: [`VkDescriptorType`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorType.html) enum value;
 * **`shader_stage_flags`**: [`VkShaderStageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderStageFlags.html) enum value which defines the shader stage where the descriptor set has to be bound;
 * **`p_descriptor_set_layout_binding`**: valid pointer to a [`VkDescriptorSetLayoutBinding`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayoutBinding.html) structure;
  **``p_descriptor_set_layout``**: valid pointer to a [`VkDescriptorSetLayout`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayout.html) handle.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    //create descriptor buffer

    VkDescriptorSetLayoutBinding set_layout_binding;
    VkDescriptorSetLayout set_layout;

    shDescriptorSetLayout(
        core.device, 
        0,
        VK_DESCRIPTOR_TYPE_UNIFORM_BUFFER,
        VK_SHADER_STAGE_VERTEX_BIT, 
        &set_layout_binding, 
        &set_layout
    );


    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

layout (set = 0, binding = 0) uniform uniformBuffer {
    // [...]
} ubo;

// [...]
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateDescriptorPool
```c
extern void shCreateDescriptorPool(VkDevice device, const VkDescriptorType descriptor_type, VkDescriptorPool* p_descriptor_pool);
```

### Description
Creates a [`VkDescriptorPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorPool.html) handle. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_type`**: [`VkDescriptorType`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorType.html) enum value;
 * **`p_descriptor_pool`**: valid pointer to a [`VkDescriptorPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorPool.html) handle.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    //create descriptor buffer

    VkDescriptorSetLayoutBinding set_layout_binding = { 0 };

    //setup descriptor set layout

    VkDescriptorPool descriptor_pool;

    shCreateDescriptorPool(
        core.device, 
        set_layout_binding.descriptorType, 
        &descriptor_pool
    );


    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shAllocateDescriptorSet
```c
extern void shAllocateDescriptorSet(VkDevice device, const uint32_t binding, VkDescriptorType descriptor_type, VkDescriptorSetLayout* p_descriptor_set_layout, VkDescriptorPool descriptor_pool, VkDescriptorSet* p_descriptor_set, VkDescriptorBufferInfo* p_buffer_info, VkWriteDescriptorSet* p_write_descriptor_set);
```

### Description
Allocates a [`VkDescriptorSet`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSet.html) handle and fills a [`VkWriteDescriptorSet`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkWriteDescriptorSet.html) structure.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`binding`**:  binding number of the entry and corresponds to a resource of the same binding number in the shader stages, see [`shPipelineBindDescriptorBufferMemory`](#shpipelinebinddescriptorbuffermemory);
 * **`descriptor_type`**: [`VkDescriptorType`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorType.html) enum value;
 * **``p_descriptor_set_layout``**: valid [`VkDescriptorSetLayout`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayout.html) pointer, see [`shDescriptorSetLayout`](#shdescriptorsetlayout);
 * **`descriptor_pool`**: valid [`VkDescriptorPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorPool.html) handle, see [`shCreateDescriptorPool`](#shcreatedescriptorpool);
 * **`p_descriptor_set`**: valid pointer to a [`VkDescriptorSet`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSet.html) handle;
 * **`p_buffer_info`** valid pointer to a [`VkDescriptorBufferInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorBufferInfo.html) structure;
 * **`p_write_descriptor_set`** valid pointer to a [`VkWriteDescriptorSet`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkWriteDescriptorSet.html) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    //create descriptor buffer

    VkDescriptorSetLayoutBinding set_layout_binding = { 0 };
    VkDescriptorSetLayout set_layout;
    VkDescriptorPool descriptor_pool;

    //setup descriptor set layout
    //create descriptor pool

    VkDescriptorSet descriptor_set;
    VkDescriptorBufferInfo descriptor_buffer_info   = { 0 };
    VkWriteDescriptorSet write_descriptor_set       = { 0 };
    
    shAllocateDescriptorSet(
        core.device,
        0,
        set_layout_binding.descriptorType,
        &set_layout,
        descriptor_pool,
        &descriptor_set,
        &descriptor_buffer_info,
        &write_descriptor_set
    );


    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateShaderModule
```c
extern void shCreateShaderModule(const VkDevice device, const uint32_t size, const char* code, VkShaderModule* p_shader_module);
```

### Description
Creates a shader module. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`size`**: size in bytes of the [`SPIR-V`](https://www.khronos.org/spir/) shader module;
 * **`code`**: shader module code;
 * **``p_shader_module``**: valid pointer to a [`VkShaderModule`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderModule.html) handle. 
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

#ifdef _MSC_VER
#pragma warning (disable: 4996)
#endif//_MSC_VER
#include <stdlib.h>
const char* readBinary(const char* path, uint32_t* p_size) {
	FILE* stream = fopen(path, "rb");
	if (stream == NULL) {
		return NULL;
	}
	fseek(stream, 0, SEEK_END);
	uint32_t code_size = ftell(stream);
	fseek(stream, 0, SEEK_SET);
	char* code = (char*)calloc(1, code_size);
	if (code == NULL) {
		fclose(stream);
		return NULL;
	}
	fread(code, code_size, 1, stream);
	*p_size = code_size;
	fclose(stream);
	return code;
}

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    uint32_t shader_size = 0;

    const char* shader_code = readBinary(
        "path/to/shader_module", 
        &shader_size
    );

    VkShaderModule shader_module;

    shCreateShaderModule(core.device, shader_size, shader_code, &shader_module);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shCreateShaderStage
```c
extern void shCreateShaderStage(const VkDevice device, const VkShaderModule shader_module, const VkShaderStageFlags shader_stage_flag, VkPipelineShaderStageCreateInfo* p_shader_stage);
```

### Description
Creates a shader stage. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`shader_module`**: valid [`VkShaderModule`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderModule.html) handle, see [`shCreateShaderModule`](#shcreateshadermodule);
 * **`shader_stage_flag`**: [`VkShaderStageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderStageFlags.html) enum value;
 * **``p_shader_stage``**: valid pointer to a [`VkPipelineShaderStageCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineShaderStageCreateInfo.html) structure. 
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    VkShaderModule shader_module;
    //create shader module

    VkPipelineShaderStageCreateInfo shader_stage_create_info = { 0 };

    shCreateShaderStage(
        core.device, 
        shader_module, 
        VK_SHADER_STAGE_VERTEX_BIT, 
        &shader_stage_create_info
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetupGraphicsPipeline
```c
extern void shSetupGraphicsPipeline(VkDevice device, VkRenderPass render_pass, const ShVkFixedStates fixed_states, ShVkPipeline* p_pipeline);
```

### Description
Creates a graphics pipeline. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`render_pass`**: valid [`VkRenderPass`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkRenderPass.html) handle;
 * **`fixed_states`**: valid [`ShVkFixedStates`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/ShVkFixedStates.html) structure, see [`shSetFixedStates`](#shsetfixedstates);
 * **``p_pipeline``**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure. 
### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    //setup swapchain data
    //setup depth data
    //setup render pass

    ShVkPipeline pipeline = { 0 };

    //setup fixed states

    //[...]

    shSetupGraphicsPipeline(core.device, core.render_pass, fixed_states, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shSetupComputePipeline
```c
extern void shSetupComputePipeline(VkDevice device, ShVkPipeline* p_pipeline);
```

### Description
Creates a compute pipeline. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`render_pass`**: valid [`VkRenderPass`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkRenderPass.html) handle;
 * **`fixed_states`**: valid [`ShVkFixedStates`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/ShVkFixedStates.html) structure, see [`shSetFixedStates`](#shsetfixedstates);
 * **``p_pipeline``**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    //[...]

    shSetupComputePipeline(core.device, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shEndPipeline
```c
extern void shEndPipeline(ShVkPipeline* p_pipeline);
```

### Description
Resets some pipeline states (dynamic descriptor offsets). 

### Parameters
 * **``p_pipeline``**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    //[...]

    shEndPipeline(&pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineRelease
```c
extern void shPipelineRelease(VkDevice device, ShVkPipeline* p_pipeline);
```

### Description
Automatically destroys every active Vulkan object stored at `p_pipeline`.

### Parameters
 * **``p_pipeline``**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    //[...]

    shPipelineRelease(&pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineCreateDescriptorBuffer
```c
extern void shPipelineCreateDescriptorBuffer(const VkDevice device, const VkBufferUsageFlags buffer_usage_flag, const uint32_t descriptor_idx, const uint32_t size, ShVkPipeline* p_pipeline);
```

### Description
Creates a descriptor [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) stored at `p_pipeline`. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`buffer_usage_flag`**: some common [`VkBufferUsageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBufferUsageFlags.html) values used to create descriptor buffer are `VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT` and `VK_BUFFER_USAGE_STORAGE_BUFFER_BIT`;
 * **`descriptor_idx`**: descriptor set index;
 * **`size`**: size in bytes of the buffer;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    shPipelineCreateDescriptorBuffer(
        core.device, 
        VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT, 
        0, 
        64, 
        &pipeline
    );


    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

layout (set = 0, binding = 0) uniform uniformBuffer {
    mat4 model;
} ubo;

// [...]
```<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineCreateDynamicDescriptorBuffer
```c
extern void shPipelineCreateDynamicDescriptorBuffer(const VkDevice device, const VkBufferUsageFlagBits buffer_usage_flag, const uint32_t descriptor_idx, const uint32_t size, const uint32_t max_bindings, ShVkPipeline* p_pipeline);
```

### Description
Creates a descriptor [`VkBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBuffer.html) stored at `p_pipeline`. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`buffer_usage_flag`**: some common [`VkBufferUsageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkBufferUsageFlags.html) values used to create descriptor buffer are `VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT` and `VK_BUFFER_USAGE_STORAGE_BUFFER_BIT`;
 * **`descriptor_idx`**: descriptor set index;
 * **`size`**: size in bytes of the buffer;
 * **`max_bindings`**: maximum number of bindings for each command buffer record;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    uint32_t max_bindings = 3;

    shPipelineCreateDynamicDescriptorBuffer(
        core.device, 
        VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT, 
        0, 
        64,
        3, 
        &pipeline
    );


    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

layout (set = 0, binding = 0) uniform uniformBuffer { //applied for 3 objects
    mat4 model;
} ubo;

// [...]
```<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineAllocateDescriptorBuffersMemory
```c
extern void shPipelineAllocateDescriptorBuffersMemory(const VkDevice device, const VkPhysicalDevice physical_device, ShVkPipeline* p_pipeline);
```

### Description
Allocates memory for all the descriptors created inside a [`shVkPipeline`](#shvkpipeline) structure. 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`physical_device`**: valid physical device handle, see [`shSelectPhysicalDevice`](#shselectphysicaldevice);
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    //create descriptor buffers

    shPipelineAllocateDescriptorBuffersMemory(core.device, core.physical_device, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineDescriptorSetLayout
```c
#define shPipelineDescriptorSetLayout(device, descriptor_idx, binding, descriptor_type, shader_stage, p_pipeline)\
	shDescriptorSetLayout(device,\
		binding,\
		descriptor_type,\
		shader_stage,\
		&(p_pipeline)->descriptor_set_layout_bindings[descriptor_idx],\
		&(p_pipeline)->descriptor_set_layouts[descriptor_idx]\
	)
```

### Description
Fills a [`VkDescriptorSetLayoutBinding`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayoutBinding.html) structure and creates a [`VkDescriptorSetLayout`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSetLayout.html) object stored at `p_pipeline`. Calls [`shDescriptorSetLayout`](#shdescriptorsetlayout).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`binding`**:  binding number of the entry and corresponds to a resource of the same binding number in the shader stages, see [`shPipelineBindDescriptorBufferMemory`](#shpipelinebinddescriptorbuffermemory);
 * **`descriptor_type`**: [`VkDescriptorType`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorType.html) enum value;
 * **`shader_stage_flags`**: [`VkShaderStageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderStageFlags.html) enum value which defines the shader stage where the descriptor set has to be bound;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 }; 

    //create descriptor buffer inside the pipeline

    shPipelineDescriptorSetLayout(
        core.device,
        0, 
        0,
        VK_DESCRIPTOR_TYPE_UNIFORM_BUFFER,
        VK_SHADER_STAGE_VERTEX_BIT, 
        &pipeline
    );

    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

layout (set = 0, binding = 0) uniform uniformBuffer {
    // [...]
} ubo;

// [...]
```
<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineCreateDescriptorPool
```c
#define shPipelineCreateDescriptorPool(device, descriptor_idx, p_pipeline)\
		shCreateDescriptorPool(device,\
			(p_pipeline)->descriptor_set_layout_bindings[descriptor_idx].descriptorType,\
			&(p_pipeline)->descriptor_pools[descriptor_idx]\
		)
```

### Description
Creates a [`VkDescriptorPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorPool.html) handle stored at `p_pipeline`. Calls [`shCreateDescriptorPool`](#shcreatedescriptorpool) 

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device
    
    ShVkPipeline pipeline = { 0 };

    //create descriptor buffer inside pipeline
    //setup descriptor set layout inside pipeline

    shPipelineCreateDescriptorPool(
        core.device, 
        0, 
        &pipeline
    );


    // [...]
    return 0;
}
```



## shPipelineAllocateDescriptorSet
```c
#define shPipelineAllocateDescriptorSet(device, descriptor_idx, p_pipeline)\
	shAllocateDescriptorSet(device,\
		(p_pipeline)->descriptor_set_layout_bindings[descriptor_idx].binding,\
		(p_pipeline)->descriptor_set_layout_bindings[descriptor_idx].descriptorType,\
		&(p_pipeline)->descriptor_set_layouts[descriptor_idx],\
		(p_pipeline)->descriptor_pools[descriptor_idx],\
		&(p_pipeline)->descriptor_sets[descriptor_idx],\
		&(p_pipeline)->descriptor_buffer_infos[descriptor_idx],\
		&(p_pipeline)->write_descriptor_sets[descriptor_idx]\
	)
```

### Description
Allocates a [`VkDescriptorSet`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDescriptorSet.html) handle and fills a [`VkWriteDescriptorSet`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkWriteDescriptorSet.html) structure stored at `p_pipeline`. Calls [`shAllocateDescriptorSet`](#shallocatedescriptorset).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    //create descriptor buffer inside pipeline
    //setup descriptor set layout inside pipeline
    //setup descriptor pool inside pipeline

    shPipelineAllocateDescriptorSet(core.device, 0, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineCreateShaderModule
```c
#define shPipelineCreateShaderModule(device, size, code, p_pipeline)\
	shCreateShaderModule(device, size, code, &(p_pipeline)->shader_modules[(p_pipeline)->shader_module_count])
```

### Description
Creates a shader module stored at `p_pipeline`. Calls [`shCreateShaderModule`](#shcreateshadermodule).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`size`**: size in bytes of the [`SPIR-V`](https://www.khronos.org/spir/) shader module;
 * **`code`**: shader module code;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

#ifdef _MSC_VER
#pragma warning (disable: 4996)
#endif//_MSC_VER
#include <stdlib.h>
const char* readBinary(const char* path, uint32_t* p_size) {
	FILE* stream = fopen(path, "rb");
	if (stream == NULL) {
		return NULL;
	}
	fseek(stream, 0, SEEK_END);
	uint32_t code_size = ftell(stream);
	fseek(stream, 0, SEEK_SET);
	char* code = (char*)calloc(1, code_size);
	if (code == NULL) {
		fclose(stream);
		return NULL;
	}
	fread(code, code_size, 1, stream);
	*p_size = code_size;
	fclose(stream);
	return code;
}

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    uint32_t shader_size = 0;

    const char* shader_code = readBinary(
        "path/to/shader_module", 
        &shader_size
    );

    VkShaderModule shader_module;

    shPipelineCreateShaderModule(
        core.device,\
        shader_size,\
        shader_code,\
        &shader_module\
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineCreateShaderStage
```c
extern void shPipelineCreateShaderStage(const VkDevice device, VkShaderStageFlags shader_stage_flag, ShVkPipeline* p_pipeline);
```

### Description
Creates a shader stage stored at `p_pipeline`. Calls [`shCreateShaderStage`](#shcreateshaderstage).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`shader_module`**: valid [`VkShaderModule`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderModule.html) handle, see [`shCreateShaderModule`](#shcreateshadermodule);
 * **`shader_stage_flag`**: [`VkShaderStageFlags`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkShaderStageFlags.html) enum value;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkPipelineData.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
    //setup physical device
    //setup logical device

    ShVkPipeline pipeline = { 0 };

    //create shader module inside pipeline

    shPipelineCreateShaderStage(//same process valid with fragment and compute stages
        core.device, 
        VK_SHADER_STAGE_VERTEX_BIT,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineWriteDescriptorBufferMemory
```c
#define shPipelineWriteDescriptorBufferMemory(device, descriptor_idx, p_descriptor_buffer_data, p_pipeline)\
	shWriteMemory(device,\
		(p_pipeline)->descriptor_buffers_memory[descriptor_idx],\
		0,\
		(uint32_t)(p_pipeline)->descriptor_buffer_infos[descriptor_idx].range,\
		p_descriptor_buffer_data\
	)
```

### Description
Writes descriptor data on the GPU. Calls [shWriteMemory](#shwritememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_descriptor_buffer_data`**: pointer to the source buffer with size at least equal to `(p_pipeline)->descriptor_buffer_infos[descriptor_idx].range`;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    ShVkPipeline pipeline = { 0 };

    //create descriptor buffer inside pipeline
    //setup descriptor set layout inside pipeline
    //setup descriptor pool inside pipeline
    //allocate descriptor set inside pipeline

    // [...]

    //update descriptor set

    float src[16] = {
        1.0f, 0.0f, 0.0f, 0.0f,
        0.0f, 1.0f, 0.0f, 0.0f,
        0.0f, 0.0f, 1.0f, 0.0f,
        0.0f, 0.0f, 0.0f, 1.0f
    };
    shPipelineWriteDescriptorBufferMemory(core.device, 0, src, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---




## shPipelineWriteDynamicDescriptorBufferMemory
```c
#define shPipelineWriteDynamicDescriptorBufferMemory(device, descriptor_idx, p_descriptor_buffer_data, p_pipeline)\
	shWriteMemory(device,\
		(p_pipeline)->descriptor_buffers_memory[descriptor_idx],\
		(p_pipeline)->dynamic_descriptor_buffer_offsets[descriptor_idx],\
		(uint32_t)(p_pipeline)->descriptor_buffer_infos[descriptor_idx].range,\
		p_descriptor_buffer_data\
	)
```

### Description
Automatically writes dynamic descriptor data on the GPU at the right offset. Calls [shWriteMemory](#shwritememory). Calls [`shWriteMemory`](#shwritememory).

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_descriptor_buffer_data`**: pointer to the source buffer with size at least equal to `(p_pipeline)->descriptor_buffer_infos[descriptor_idx].range`;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    
    ShVkPipeline pipeline = { 0 };

    //create descriptor buffer inside pipeline
    //setup descriptor set layout inside pipeline
    //setup descriptor pool inside pipeline
    //allocate descriptor set inside pipeline

    // [...]

    //update descriptor set

    float src[16] = {
        1.0f, 0.0f, 0.0f, 0.0f,
        0.0f, 1.0f, 0.0f, 0.0f,
        0.0f, 0.0f, 1.0f, 0.0f,
        0.0f, 0.0f, 0.0f, 1.0f
    };
    shPipelineWriteDynamicDescriptorBufferMemory(core.device, 0, src, &pipeline);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelinePushConstants
```c
#define shPipelinePushConstants(cmd_buffer, p_push_constant_data, p_pipeline)\
	vkCmdPushConstants(cmd_buffer,\
		(p_pipeline)->pipeline_layout,\
		(p_pipeline)->push_constant_range.stageFlags,\
		(p_pipeline)->push_constant_range.offset,\
		(p_pipeline)->push_constant_range.size,\
		p_push_constant_data\
	)
```

### Description
Writes push constant data on the GPU. Calls [vkCmdPushConstants](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkCmdPushConstants.html).

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`p_push_constant_data`**: pointer to the source buffer with size at least equal to `(p_pipeline)->push_constant_range.size`;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    //setup push constant

    // [...]

    float src[32] = {
        1.0f, 0.0f, 0.0f, 0.0f,
        0.0f, 1.0f, 0.0f, 0.0f,
        0.0f, 0.0f, 1.0f, 0.0f,
        0.0f, 0.0f, 0.0f, 1.0f,

        1.0f, 0.0f, 0.0f, 0.0f,
        0.0f, 1.0f, 0.0f, 0.0f,
        0.0f, 0.0f, 1.0f, 0.0f,
        0.0f, 0.0f, 0.0f, 1.0f
    };

    uint32_t thread_idx = 0;
    shPushConstants(//same process valid with graphics pipelines
        core.compute_commands[thread_idx].cmd_buffer,
        src,
        &pipeline
    );

    // [...]
    return 0;
}
```
`GLSL` shader code:
```glsl
#version 460

//max size: 128 bytes
layout (push_constant) uniform pushConstant {
    mat4 projection;
    mat4 view;
} pconst;

// [...]
```
<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shBindPipeline
```c
#define shBindPipeline(cmd_buffer, bind_point, p_pipeline)\
	vkCmdBindPipeline(cmd_buffer, bind_point, (p_pipeline)->pipeline)
```

### Description
Binds a pipeline. Calls [`vkCmdBindPipeline`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkCmdBindPipeline.html)

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`bind_point`**: pipeline binding point, see [`VkPipelineBindPoint`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineBindPoint.html);
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    //setup push constant

    // [...]

    uint32_t thread_idx = 0;
    shBindPipeline(//same process valid with graphics pipelines
        core.compute_commands[thread_idx].cmd_buffer,
        VK_PIPELINE_BIND_POINT_COMPUTE,    
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineUpdateDescriptorSets
```c
#define shPipelineUpdateDescriptorSets(device, p_pipeline)\
	vkUpdateDescriptorSets(device,\
		(p_pipeline)->descriptor_count, 
        (p_pipeline)->write_descriptor_sets,\
		0, 
        NULL\
    )
```

### Description
Updates all active descriptor sets stored at `p_pipeline`. Calls [`vkUpdateDescriptorSets`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkUpdateDescriptorSets.html)

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    // [...]

    shPipelineUpdateDescriptorSets(
        core.device,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---




## shPipelineUpdateDescriptorSet
```c
#define shPipelineUpdateDescriptorSet(device, descriptor_idx, p_pipeline)\
	vkUpdateDescriptorSets(device,\
		1,\
		&(p_pipeline)->write_descriptor_sets[descriptor_idx],\
		0,\
		NULL\
	)
```

### Description
Updates a descriptor set stored at `p_pipeline`. Calls [`vkUpdateDescriptorSets`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkUpdateDescriptorSets.html)

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [`shSetLogicalDevice`](#shsetlogicaldevice);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    // [...]

    shPipelineUpdateDescriptorSet(
        core.device,
        0,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---




## shPipelineBindDescriptorSet
```c
#define shPipelineBindDescriptorSet(cmd_buffer, descriptor_idx, bind_point, p_pipeline)\
	vkCmdBindDescriptorSets(cmd_buffer,\
		bind_point,\
		(p_pipeline)->pipeline_layout,\
		descriptor_idx,\
		1,\
		&(p_pipeline)->descriptor_sets[descriptor_idx],\
		0,\
		NULL\
	)
```

### Description
Binds a descriptor set stored at `p_pipeline`. Calls [`vkCmdBindDescriptorSets`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkCmdBindDescriptorSets.html).

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`descriptor_idx`**: descriptor set index;
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    // [...]

    //update descriptor
    //write descriptor set memory

    uint32_t thread_idx = 0;
    shPipelineBindDescriptorSet(//same process valid with graphics pipelines
        core.compute_commands[0].cmd_buffer,
        core.device,
        0,
        VK_PIPELINE_BIND_POINT_COMPUTE,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---




## shPipelineBindDescriptorSets
```c
#define shPipelineBindDescriptorSets(cmd_buffer, first_descriptor, descriptor_count, bind_point, p_pipeline)\
	vkCmdBindDescriptorSets(cmd_buffer,\
		bind_point,\
		(p_pipeline)->pipeline_layout,\
		first_descriptor,\
		descriptor_count,\
		&(p_pipeline)->descriptor_sets[first_descriptor],\
		0,\
		NULL\
	)
```

### Description
Binds all the descriptor sets stored at `p_pipeline` specified with the range `first_descriptor` : `descriptor_count`. Calls [`vkCmdBindDescriptorSets`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkCmdBindDescriptorSets.html).

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`first_descriptor`**: index of the first descriptor to bind;
 * **`descriptor_count`**: total number of descriptors to bind;
 * **`bind_point`**: pipeline binding point, see [`VkPipelineBindPoint`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineBindPoint.html);
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    // [...]

    //update descriptors
    //write descriptor sets memory

    uint32_t thread_idx = 0;
    shPipelineBindDescriptorSets(//same process valid with graphics pipelines
        core.compute_commands[0].cmd_buffer,
        core.device,
        0
        3,//you should have created three descriptor sets
        VK_PIPELINE_BIND_POINT_COMPUTE,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineBindDynamicDescriptorSet
```c
extern void shPipelineBindDynamicDescriptorSet(const VkCommandBuffer cmd_buffer, const uint32_t descriptor_idx, const VkPipelineBindPoint bind_point, ShVkPipeline* p_pipeline);
```

### Description
Binds a dynamic descriptor set stored at `p_pipeline`. Calls [`vkCmdBindDescriptorSets`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkCmdBindDescriptorSets.html). The descriptor buffer offset automatically increases by the size of the descriptor sets.

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`descriptor_idx`**: descriptor set index;
 * **`bind_point`**: pipeline binding point, see [`VkPipelineBindPoint`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineBindPoint.html);
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    // [...]

    //update descriptor
    //write descriptor set memory

    uint32_t thread_idx = 0;
    shPipelineBindDynamicDescriptorSet(//same process valid with graphics pipelines
        core.compute_commands[0].cmd_buffer,
        core.device,
        0,
        VK_PIPELINE_BIND_POINT_COMPUTE,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shPipelineBindDynamicDescriptorSets
```c
extern void shPipelineBindDynamicDescriptorSets(const VkCommandBuffer cmd_buffer, const uint32_t first_descriptor, const uint32_t descriptor_count, const VkPipelineBindPoint bind_point, ShVkPipeline* p_pipeline);
```

### Description
Binds all the dynamic descriptor sets stored at `p_pipeline` specified with the range `first_descriptor` : `descriptor_count`. Calls [`vkCmdBindDescriptorSets`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/vkCmdBindDescriptorSets.html). The descriptor buffer offset automatically increases by the size of the descriptor sets.

### Parameters
 * **`cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers) and [`shBeginCommandBuffer`](#shbegincommandbuffer);
 * **`first_descriptor`**: index of the first descriptor to bind;
 * **`descriptor_count`**: total number of descriptors to bind;
 * **`bind_point`**: pipeline binding point, see [`VkPipelineBindPoint`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkPipelineBindPoint.html);
 * **`p_pipeline`**: valid pointer to a [`ShVkPipeline`](#shvkpipeline) structure.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    // [...]

    //update descriptors
    //write dynamic descriptor sets memory

    uint32_t thread_idx = 0;
    shPipelineBindDynamicDescriptorSets(//same process valid with graphics pipelines
        core.compute_commands[0].cmd_buffer,
        core.device,
        0
        3,//you should have created three dynamic descriptor sets
        VK_PIPELINE_BIND_POINT_COMPUTE,
        &pipeline
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## SH_VULKAN_GENERATE_DESCRIPTOR_STRUCTURE_MAP
```c
#define SH_VULKAN_GENERATE_DESCRIPTOR_STRUCTURE_MAP(STRUCT)\
    // [...]
```

### Description
Macro definition which generates some utility functions that map a specific structure array according to the GPU minumum uniform buffer offset alignment.

### Parameters
 * **`STRUCT`**: structure typename.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>
#include <shvulkan/shVkDescriptorStructureMap.h>

#ifndef alignas
#include "../../external/stdalign.in.h"
#endif//alignas

typedef struct Model {
	alignas(16) float model[4][4];
} Model;
SH_VULKAN_GENERATE_DESCRIPTOR_STRUCTURE_MAP(Model) //required only for dynamic descriptors

#include <stdlib.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    ShVkPipeline pipeline = { 0 };

    uint32_t model_count = 2;

    float src[4][4] = {
		1.0f, 0.0f, 0.0f, 0.0f,
		0.0f, 2.0f, 0.0f, 0.0f,
		0.0f, 0.0f, 1.0f, 0.0f,
		0.0f, 0.0f, 0.0f, 1.0f
	};

	ModelDescriptorStructureMap map = shVkCreateModelDescriptorStructures(
        core.physical_device_properties, 
        model_count
    );

	Model* p_model_0 = shVkGetModelDescriptorStructure(model_map, 0, 0);
	Model* p_model_1 = shVkGetModelDescriptorStructure(model_map, 1, 0);

	memcpy(p_model_0->model, src, 64);
	memcpy(p_model_1->model, src, 64);

	shVkMapModelDecriptorStructures(&map);

	shPipelineCreateDynamicDescriptorBuffer(
        core.device, 
        VK_BUFFER_USAGE_UNIFORM_BUFFER_BIT, 
        0, 
        map.structure_size,
        model_count,
        &pipeline
    );

    shPipelineAllocateDescriptorBufferMemory(
        core.device, 
        core.physical_device, 
        0, 
        &pipeline
    );

    shPipelineBindDescriptorBufferMemory(core.device, 0, &pipeline);

    shPipelineDescriptorSetLayout(
        core.device, 
        0, 
        0, 
        VK_DESCRIPTOR_TYPE_UNIFORM_BUFFER_DYNAMIC, 
        VK_SHADER_STAGE_VERTEX_BIT, 
        &pipeline
    );

    // [...]
    return 0;
}
```
`GLSL` shader code:
```
#version 460

layout (set = 0, binding = 0) uniform uniformBuffer {
    mat4 model;
} ubo;

// [...]
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shGetDescriptorSize
```c
static uint32_t shGetDescriptorSize(ShVkCore* p_core, uint32_t _size);
```

### Description
Returns the size of a descriptor set according to the GPU minumum uniform buffer offset alignment.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`size`**: initial descriptor size.

### Usage example

```c
#include <shvulkan/shVkDescriptorStructureMap.h>

#ifndef alignas
#include "../../external/stdalign.in.h"
#endif//alignas

typedef struct Model {
	alignas(16) float model[4][4];
} Model;

#include <stdlib.h>

int main(void) {
    
    ShVkCore* p_core;
    //setup instance
    //setup physical device

    uint32_t descriptor_size = shGetDescriptorSize(p_core, sizeof(Model));

    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shFrameReset
```c
extern void shFrameReset(ShVkCore* p_core, uint32_t thread_idx);
```

### Description
Given a thread index, resets a command buffer and a fence.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`thread_idx`**: thread index.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>
#include <shvulkan/shVkDescriptorStructureMap.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers
    //create surface --> platform dependent
    //setup swapchain
    //get swapchain images
    //get swapchain image views
    //setup render pass

    // [...]

    uint32_t thread_idx = 0;

    shFrameReset(&core, thread_idx);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shFrameBegin
```c
extern void shFrameBegin(ShVkCore* p_core, const uint32_t thread_idx, uint32_t* p_swapchain_image_idx);
```

### Description
Acquires an image ready for presenting and records a command buffer.

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`thread_idx`**: thread index;
 * **`p_swapchain_image_idx`**: image index pointer.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>
#include <shvulkan/shVkDescriptorStructureMap.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers
    //create surface --> platform dependent
    //setup swapchain
    //get swapchain images
    //get swapchain image views
    //setup render pass

    // [...]

    uint32_t thread_idx = 0;
    uint32_t image_idx = 0;

    shFrameBegin(&core, thread_idx, &image_idx);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shDrawIndexed
```c
#define shDrawIndexed(graphics_cmd_buffer, index_count)\
	vkCmdDrawIndexed(graphics_cmd_buffer, index_count, 1, 0, 0, 0)
```

### Description
Records an indexed draw call.

### Parameters
 * **`graphics_cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers);
 * **`index_count`**: number of mesh indices.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>
#include <shvulkan/shVkDescriptorStructureMap.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    uint32_t quad_index_count = 6;

    // [...]

    uint32_t thread_idx = 0;
    shDrawIndexed(&core.graphics_commads[thread_idx].cmd_buffer, quad_index_count);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shDraw
```c
#define shDraw(graphics_cmd_buffer, vertex_count_div_stride)\
    vkCmdDraw(graphics_cmd_buffer, vertex_count_div_stride, 1, 0, 0)
```

### Description
Records a draw call.

### Parameters
 * **`graphics_cmd_buffer`**: recording [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [`shCreateGraphicsCommandBuffers`](#shcreategraphicscommandbuffers) and [`shCreateComputeCommandBuffers`](#shcreatecomputecommandbuffers);
 * **`vertex_count_div_stride`**: number of vertices divided by the vertex stride.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>
#include <shvulkan/shVkDescriptorStructureMap.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    uint32_t vertex_count = 24;
    float vertices[24] = {
			-1.0f, 1.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f,
			 0.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f,
			 1.0f, 1.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f, 0.0f
	};


    ShVkFixedStates fixed_states = { 0 };

    shSetVertexInputAttribute(0, SH_VEC3_SIGNED_FLOAT, 0, 12 &fixed_states);
	shSetVertexInputAttribute(1, SH_VEC3_SIGNED_FLOAT, 12, 12, &fixed_states);
	shSetVertexInputAttribute(2, SH_VEC2_SIGNED_FLOAT, 24, 8, &fixed_states);

    // [...]


    uint32_t thread_idx = 0;
    shDraw(
        &core.graphics_commads[thread_idx].cmd_buffer, 
        vertex_count / (fixed_states.vertex_binding_description.stride / sizeof(uint32_t)),
    );

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---



## shFrameEnd
```c
extern void shFrameEnd(ShVkCore* p_core, const uint32_t thread_idx, const uint32_t swapchain_image_idx);
```

### Description

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`thread_idx`**: thread index;
 * **`swapchain_image_idx`**: image index.

### Usage example

```c
#include <shvulkan/shVkCore.h>
#include <shvulkan/shVkMemoryInfo.h>
#include <shvulkan/shVkDescriptorStructureMap.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    //setup logical device
    //setup command buffers

    // [...]

    uint32_t thread_idx = 0;
    uint32_t image_idx = 0;

    //begin frame

    shFrameEnd(core.graphics_commands[thread_idx].cmd_buffer, image_idx);

    // [...]
    return 0;
}
```

<button class="btn">[top](#shvulkan-c-definitions)</button>

---




<button class="btn">[back to docs](./index)</button>