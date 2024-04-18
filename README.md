# ComfyUI StabilityAI Suite

This fork of the official StabilityAI repository contains a number of enhancements and implementations.

## Image Core + Style Preset

In the official version there is no option to set one of the available __styles__. In this fork the node has been updated: it contains a new true/false switch to activate styles, and the corresponding selector.

![Image Core + Style Preset](/images/image_core_style.png)

## Creative Upscale Recover File 

The node for the creative uspcale performs two steps: generation and recovery of the generated image. If unfortunately your PC has a crash or suddenly lacks an Internet connection, the second step cannot complete and you risk losing the generated image and the credits used. Fortunately, the images are archived for 24 hours by StabilityAI.
Thanks to a change in the general code, the  unique __id__ are automatically saved within the __log.txt__ file. This file is automatically created and saved in the same folder as the custom node. Follow these steps now:

- Open the file and copy the desired `id`.
- Paste the `id` into the __Creative Upscale Recover File__ node to recover the lost image.

![Creative Upscale Recover File](/images/creative_upscale_recover_file.png)

## Usage:

Add API key to environment variable "`SAI_API_KEY`".

Alternatively you can write your API key to file "`sai_platform_key.txt`".

You can also use and/or override the above by entering your API key in the '`api_key_override`' field of each node.

## Other projects

- [ComfyUI Portrait Master](https://github.com/florestefano1975/comfyui-portrait-master/)
- [ComfyUI Prompt Composer](https://github.com/florestefano1975/comfyui-prompt-composer/)