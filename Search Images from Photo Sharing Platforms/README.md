# [Free Automated Image Search from Photo Sharing Platforms](https://burstyai.com)

## How to Use This Tool

This tool helps you find and select images from popular platforms like Unsplash, Pixabay, and Pexels. Here's how to use it:

1. **Define Search Keywords**:
   - Input relevant keywords that describe the type of images you need. These keywords will be used to search for images on the selected platforms.

2. **Set Image Parameters**:
   - Choose the desired image size ratio from options like 4:3 (standard), 1:1 (square), 16:9 (widescreen), and 3:2.
   - Specify the number of images you want to select from the search results. The default is set to 3, but you can customize this based on your needs.

3. **Run the Workflow**:
   - Execute the workflow through the interactive form. The tool will refine your keywords, conduct the search, and select the top images based on relevance and your criteria.

4. **Review and Download Results**:
   - View the selected images directly on the BurstyAI platform.
   - Download the image URLs and descriptions as a CSV file for your records.

## How It Works

The Image Search workflow operates in several steps:

1. **Refine Search Keywords**:
   - The tool uses a language model to generate 1-3 relevant search keywords based on your input, ensuring compatibility with platforms like Unsplash, Pixabay, and Pexels.

2. **Search Images from Platforms**:
   - It conducts the search using the refined keywords, filtering results by the specified image size ratio to match your layout requirements.

3. **Select Top Images**:
   - The tool uses a language model to choose the top N images based on relevance, description, and some level of randomization. This ensures a good mix of highly relevant images and a few varied options.

## FAQs

> **Q: How do I input the search keywords?**
> **A:** Enter the keywords in the "Image Search Keywords" field in the interactive form. These keywords should describe the type of images you are looking for.

> **Q: What image size ratios can I choose?**
> **A:** You can select from 4:3 (standard), 1:1 (square), 16:9 (widescreen), and 3:2. This ensures the images fit your specific layout requirements.

> **Q: How many images can I select?**
> **A:** You can specify the number of images to select in the "Number of Images" field. The default is 3, but you can increase or decrease this number as needed.

> **Q: Can I download the results?**
> **A:** Yes, you can download the image URLs and descriptions as a CSV file from the BurstyAI platform.

> **Q: How are the top images selected?**
> **A:** The tool uses a language model to select images based on relevance to your keywords and descriptions, with some randomization to provide a varied selection.

# Search Images from Photo Sharing Platforms API

This API endpoint searches for images on platforms like Unsplash, Pixabay, and Pexels based on specified keywords. It refines the search results according to user-defined criteria such as aspect ratio and the number of images.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/66013e679a905a000161f68f/async_run`

### Method
`POST`

## Description

This workflow conducts image searches on popular photo-sharing platforms using provided keywords. It allows for the specification of the aspect ratio and number of images to be retrieved, helping users find images that meet specific criteria.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `Yf5hWc###image_search_keywords` (string, required): Keywords for searching images on Unsplash, Pixabay, and Pexels.
  - `Yf5hWc###image_size_ratio` (string, required): The desired aspect ratio for the images. Options include 4:3 (standard), 1:1 (square), 16:9 (widescreen), and 3:2.
  - `Yf5hWc###image_amount` (string, required): The number of images to be retrieved.

### Example JSON Request

```json
{
  "params": {
    "Yf5hWc###image_search_keywords": "nature landscapes",
    "Yf5hWc###image_size_ratio": "16/9",
    "Yf5hWc###image_amount": "5"
  }
}
