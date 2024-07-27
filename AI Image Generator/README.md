# [Free and Automated AI Image Generator](https://burstyai.com)

## How to Use This Tool

The AI Image Generator is designed to help you create stunning images from text prompts. Here's how you can use it:

1. **Enter Your Prompt**: Provide a detailed description of the image you want to generate.
2. **Select an Image Model**: Choose from various models like DALLE.2, DALLE.3, or Stable Diffusion XL versions.
3. **Set Image Details**:
   - **Amount**: Specify the number of images you need.
   - **Size**: Choose the image size (e.g., 1024x1024, 512x512).
   - **Negative Prompt**: List any traits to avoid, like "cartoon" or "blurry."
4. **Generate Images**: Click the generate button and let the AI create your images.
5. **Review and Save**: Once generated, you can review the images, save them to a sheet, or download them as a CSV file.

## How It Works

The AI Image Generator operates through a few simple steps:

- **Text Input**: You start by inputting a detailed description or prompt.
- **Model Selection**: The tool lets you choose from multiple advanced AI models:
  - **DALLE.2**: Known for its impressive ability to generate diverse and high-quality images.
  - **DALLE.3**: Offers improved realism and detail over its predecessors.
  - **Stable Diffusion Versions**: Provides a range of styles and artistic variations, from realistic to abstract.
- **Parameter Settings**: Customize your image by setting parameters like size, quantity, and negative prompts to avoid unwanted features.
- **Image Generation**: The AI processes your input and generates images based on the selected parameters.
- **Output Options**: Save the images to your BurstyAI platform sheet or download them for offline use.

## FAQs

> **Q: How do I embed the image generator form on my website?**  
> A: You can embed the form using an iframe code provided in the tool settings.

> **Q: Can I use my own images for the AI to modify?**  
> A: Yes, you can use the "Source Image" and "Mask Image" options for image-to-image or inpainting operations.

> **Q: Is there a limit to the number of images I can generate?**  
> A: While there are no strict limits, the free subscription plan allows a generous number of images per session.

> **Q: How can I avoid unwanted traits in my images?**  
> A: Use the "Negative Prompt" option to specify traits or styles you want to exclude from the generated images.

# AI Image Generator API

The "AI Image Generator" API creates images based on textual prompts using various image models such as DALLE.2, DALLE.3, and Stable Diffusion versions. It allows users to specify the image model, size, quantity, and exclude certain traits like cartoon or blurry effects.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/6624f15df5eecc0001383aa3/async_run`

### Method
`POST`

## Description

This API generates images based on provided textual prompts. Users can choose from multiple AI models, specify the number and size of images, and define traits to avoid in the images. The workflow supports various generation operations, including text-to-image, image-to-image, and inpainting.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `pNXO4A###BURSTYAI_LLM_QUERY_PROMPT` (string, required): A detailed description or prompt to guide the AI in generating images.
  - `pNXO4A###BURSTYAI_LLM_IMAGE_MODEL` (string, required): The model to use for generating images. Different models offer variations in style, realism, and prompt adherence.
  - `pNXO4A###BURSTYAI_LLM_IMAGE_AMOUNT` (string, optional): The number of images to generate. Default is 3.
  - `pNXO4A###BURSTYAI_LLM_IMAGE_SIZE` (string, optional): The size of the generated images. Options vary by model.
  - `pNXO4A###BURSTYAI_IMAGE_GEN_OPERATION` (string, optional): The type of image generation operation (e.g., text-to-image, image-to-image, inpainting). Default is "text-to-image".
  - `pNXO4A###BURSTYAI_LLM_NEGATIVE_PROMPT` (string, optional): Descriptive terms to avoid in the image generation (e.g., "Disfigured, cartoon, blurry").
  - `pNXO4A###BURSTYAI_SOURCE_IMAGE_URI` (string, optional): For image-to-image or inpainting operations, the URI of the source image.
  - `pNXO4A###BURSTYAI_MASK_IMAGE_URI` (string, optional): For inpainting operations, the URI of the mask image to indicate areas to fill or alter.

### Example JSON Request

```json
{
  "params": {
    "pNXO4A###BURSTYAI_LLM_QUERY_PROMPT": "A serene landscape with mountains and a river",
    "pNXO4A###BURSTYAI_LLM_IMAGE_MODEL": "realistic-vision-v5-1",
    "pNXO4A###BURSTYAI_LLM_IMAGE_AMOUNT": "2",
    "pNXO4A###BURSTYAI_LLM_IMAGE_SIZE": "1024x768",
    "pNXO4A###BURSTYAI_IMAGE_GEN_OPERATION": "text-to-image",
    "pNXO4A###BURSTYAI_LLM_NEGATIVE_PROMPT": "Disfigured, cartoon, blurry"
  }
}
