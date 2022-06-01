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

[Functions and macros](#functions-and-macros):
* Defined at [`shVkCheck.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCheck.h):
    * [shCheckValidationLayers](#shcheckvalidationlayers)
    * [shTranslateVkResult](#shtranslatevkresult)
    * [shVkAssertResult](#shvkassertresult)
    * [shVkAssert](#shvkassert)
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
    return 0;
}
```



---



## shTranslateVkResult
```c
extern const char* shTranslateVkResult(const VkResult vk_result);
```
### Description
Translates a `VkResult` returned by calling a Vulkan API function. Returns the literal translation of [`vk_result`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html).

### Parameters
 * [**`vk_result`**](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html).

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
    return 0;
}
```



---



## shVkAssertResult
```c
#define shVkAssertResult(result, error_msg)\
    if ((VkResult)(result) != VK_SUCCESS) {\
    		printf("shvulkan error: %s, %s\n", error_msg, shTranslateVkResult((VkResult)(result)));\
    		assert((VkResult)(result) == VK_SUCCESS);\
    	}\
```
### Description
Asserts a [`VkResult`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkResult.html)

### Parameters
 * **`result`**: an input `VkResult`;
 * **`error_msg`**: the message (encoded in a `const char*`) to display on the console when the `result` is not equal to `VK_SUCCESS`.  

### Usage example
```c
#include <shvulkan/shVkCheck.h>ì
#include <stdio.h>

int main(void) {
    VkInstance instance = NULL;
    VkInstanceCreateInfo instance_create_info = { 0 };
    shVkAssertResult(
        vkCreateInstance(&instance_create_info, NULL, &instance),
        "invalid instance create info structure"
    );
    return 0;
}
```



---



## shVkAssert
```c
#define shVkAssert(condition, error_msg)\
	assert((int)(condition) &&\
	"shvulkan error: " &&\
	(const char*)(error_msg))
```
### Description
Asserts a `condition` value, automatically casted to a signed integer.

### Parameters
 * **`condition`**;
 * [**`error_msg`**](#gaiauniversemodelmemory): the message (encoded in a `const char*`) to display on the console when the `condition` is lower or equal to zero. 

### Usage example
```c
#include <shvulkan/shVkCheck.h>ì

int main(void) {
    shVkAssert(0, "failure");
    return 0;
}
```



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

	return 0;
}
```



---



## shSelectPhysicalDevice
```c
extern void shSelectPhysicalDevice(ShVkCore* p_core, const VkQueueFlags requirements);
```
### Description
Picks a physical device given a valid [`ShVkCore`](#shvkcore) structure and some requirement flags.

### Parameters
 * **`p_core`**: the instance must have been successfully created with [`shCreateInstance`](#shcreateinstance);
 * **`requirements`**: flags to filter the GPUs that support graphics `SH_VK_CORE_GRAPHICS` or compute operations `SH_VK_CORE_COMPUTE`;

### Usage example
```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	shSelectPhysicalDevice(&core, SH_VK_CORE_GRAPHICS | SH_VK_CORE_COMPUTE);
    return 0;
}
```



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


---


## shSetLogicalDevice
```c
extern void shSetLogicalDevice(ShVkCore* p_core, VkQueueFlags requirements);
```
### Description
Creates a logical device ([`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html)). 

### Parameters
 * **`p_core`**: valid pointer to a [`ShVkCore`](#shvkcore) structure;
 * **`requirements`**: requirement flags for setting up graphics and compute[`VkDeviceQueueCreateInfo`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDeviceQueueCreateInfo.html).

### Usage example
```c
#include <shvulkan/shVkCore.h>

int main(void) {
    ShVkCore core = { 0 };
    //setup instance
	//setup physical device
    shSetLogicalDevice(&core, SH_VK_CORE_GRAPHICS | SH_VK_CORE_COMPUTE);
    return 0;
}
```



---


