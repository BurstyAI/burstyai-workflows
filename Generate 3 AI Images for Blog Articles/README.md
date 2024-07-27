# [Free Automated Tool to Generate 3 AI Images for Blog Articles](https://burstyai.com)

## How to Use This Tool

Using the "Generate 3 AI Images for Blog Articles" workflow is simple and user-friendly. Here’s how you can create stunning images for your blog articles in no time:

1. **Start by providing the blog article title**: This will help the tool understand the theme and generate relevant prompts.
2. **Run the workflow**: The tool will create three detailed prompts based on your input and generate high-quality images.
3. **Review and download your images**: Once generated, you can save the images to a sheet in the platform or download them as a CSV file.
4. **Embed the images**: You can easily embed the generated images into any website using an iframe embedding code provided by the tool.

This process ensures that the visuals created are perfectly aligned with the theme and content of your blog article.

## How It Works

The workflow operates through the following steps:

1. **Generate Image Generation Prompts**: The tool first crafts three detailed prompts based on the blog title you provide. These prompts guide the AI in creating images that match your article's theme.
2. **Define Workflow Parameters**: The tool sets up the parameters needed for the workflow, ensuring each step has the necessary information.
3. **LLM Generate Images**: Using advanced AI models, the tool generates realistic images based on the prompts. It filters out any unrealistic elements to ensure high-quality outputs.
4. **Define Workflow Outputs**: Finally, the generated images are prepared for download or embedding, with appropriate alt text for accessibility.

By following these steps, the tool ensures that the images generated are not only visually appealing but also relevant to your content.

## FAQs

> **Q: How do I start using this tool?**  
> A: Simply enter the title of your blog article into the provided field and run the workflow.

> **Q: Can I customize the generated prompts?**  
> A: Yes, the tool allows you to modify the prompts if needed, to better suit your specific needs.

> **Q: How can I integrate the generated images into my website?**  
> A: Use the provided iframe embedding code to seamlessly integrate the images into your website.

> **Q: What formats are the images available in?**  
> A: The images can be saved to a sheet in the platform or downloaded as a CSV file.

# Generate 3 AI Images for Blog Articles API

This API workflow generates three AI-created images specifically for blog articles. It starts by crafting detailed prompts based on the blog title and uses these prompts to create high-quality images that align with the article's theme.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/664245595d00f000010eb663/async_run`

### Method
`POST`

## Description

The workflow generates three AI images for use in blog articles, guided by the blog post title. This ensures that each image visually complements the theme and content of the article, enhancing the overall presentation.

## Request Body

The request body must be a JSON object containing the following field:

- `params`: Object containing the required parameter.
  - `BqNtRV###BURSTYAI_LLM_QUERY_PROMPT` (string, required): The title of the blog post or article, which will guide the image generation process.

### Example JSON Request

```json
{
  "params": {
    "BqNtRV###BURSTYAI_LLM_QUERY_PROMPT": "The Future of AI in Everyday Life"
  }
}

