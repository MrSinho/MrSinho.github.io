# shvulkan c definitions

<button>[back to index](./index)</button>

[Types and structures](#types-and-structures):
* Defined at [`shVkCore.h`](https://github.com/MrSinho/shvulkan/blob/main/shvulkan/include/shvulkan/shVkCore.h)
    * [ShVkCore](#shvkcore)
    * [ShVkSurface](#shvksurface)
    * [ShVkQueue](#shvkqueue)
    * [ShVkCommand](#shvkcommand)
    * [ShVkImageType](#shvkimagetype)
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



## ShVkImageType
```c
typedef enum ShVkImageType {
	SH_SWAPCHAIN_IMAGE = 0b001,
	SH_DEPTH_IMAGE = 0b010
} ShVkImageType;
```
### Description
Enum type required to define the usage of a specific [`VkImage`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkImage.html).



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
    // [...]
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
    // [...]
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
 * **`condition`**: the input value that ignites assertion;
 * [**`error_msg`**](#gaiauniversemodelmemory): the message (encoded in a `const char*`) to display on the console when the `condition` is lower or equal to zero. 

### Usage example
```c
#include <shvulkan/shVkCheck.h>ì

int main(void) {
    shVkAssert(0, "failure");
    // [...]
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

	// [...]
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
    // [...]
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
    // [...]
    return 0;
}
```



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



---



## shRenderPassRelease
```c
extern void shRenderPassRelease(ShVkCore* p_core);
```
### Description
Destroys the [VkRenderPass](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkRenderPass.html) stored at `p_core`.
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



---



## shInstanceRelease
```c
extern void shInstanceRelease(ShVkCore* p_core);
```
### Description
Destroys the [VkInstance](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkInstance.html) stored at `p_core`.
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



---



## shCreateGraphicsCommandBuffers

```c
#define shCreateGraphicsCommandBuffers(p_core, thread_count)\
	shCreateCommandData(p_core, VK_QUEUE_GRAPHICS_BIT, thread_count, &(p_core)->p_graphics_commands)\
```
### Description
Builds a `thread_count` number of graphics [`VkCommandPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandPool.html)s and [VkCommandBuffer](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html)s.

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



---



## shCreateComputeCommandBuffers

```c
#define shCreateComputeCommandBuffers(p_core, thread_count)\
	shCreateCommandData(p_core, VK_QUEUE_COMPUTE_BIT, thread_count, &(p_core)->p_compute_commands)\
```
### Description
Builds a `thread_count` number of compute [`VkCommandPool`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandPool.html)s and [VkCommandBuffer](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html)s.

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



---



## shBeginCommandBuffer
```c
extern void shBeginCommandBuffer(const VkCommandBuffer cmd_buffer);
```
### Description
Starts recording a [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html).

### Parameters
 * **`cmd_buffer`**: valid [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [shCreateGraphicsCommandBuffers](#shcreategraphicscommandbuffers) and [shCreateComputeCommandBuffers](#shcreatecomputecommandbuffers).

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



---



## shQueueSubmit
```c
extern void shQueueSubmit(VkCommandBuffer* cmd_buffer, const VkQueue queue, VkFence fence);
```
### Description
Submits rendering data to the GPU. 

### Parameters
 * **`cmd_buffer`**: valid [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [shCreateGraphicsCommandBuffers](#shcreategraphicscommandbuffers) and [shCreateComputeCommandBuffers](#shcreatecomputecommandbuffers).

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



---



## shCmdDispatch
```c
#define shCmdDispatch(cmd_buffer, group_count_x, group_count_y, group_count_z) vkCmdDispatch(cmd_buffer, group_count_x, group_count_y, group_count_z)
```
### Description
Dispatches compute work groups along x, y, and z dimensions. 

### Parameters
 * **`cmd_buffer`**: valid [`VkCommandBuffer`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkCommandBuffer.html), see [shCreateComputeCommandBuffers](#shcreatecomputecommandbuffers);
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



---



## shWaitForFences
```c
#define shWaitForFences(device, fence_count, p_fences) vkWaitForFences(device, fence_count, p_fences, VK_TRUE, 100000000000)
```
### Description
Waits for a `fence_count` number of [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html)s to unlock.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [shSetLogicalDevice](#shsetlogicaldevice);
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



---



## shWaitForFence
```c
#define shWaitForFence(device, p_fence) vkWaitForFences(device, 1, p_fence, VK_TRUE, 100000000000)
```
### Description
Waits for a [`VkFence`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkFence.html) to unlock.

### Parameters
 * **`device`**: valid [`VkDevice`](https://www.khronos.org/registry/vulkan/specs/1.3-extensions/man/html/VkDevice.html), see [shSetLogicalDevice](#shsetlogicaldevice);
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



---



## shCreateDepthImageView
```c
#define shCreateDepthImageView(p_core) shCreateImageView(p_core, (p_core)->depth_image, SH_DEPTH_IMAGE, &(p_core)->depth_image_view)
```
### Description
Sets up a depth image view handle.

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
    shCreateDepthImage(&core);
    // [...]
    return 0;
}
```



---



<button>[back to index](./index)</button>