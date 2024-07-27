# [Free Automated AI Blog Images Generation & Post to WordPress](https://burstyai.com)

## How to Use This Tool

This tool helps you generate AI-crafted images based on your blog post titles and automatically uploads them to WordPress. Here's how to use it:

1. **Enter Your Blog Title**: Start by entering the title of your blog post.
2. **Generate Prompts**: The tool will create three image generation prompts relevant to your blog title.
3. **Generate Images**: Using these prompts, the AI model will generate high-quality images.
4. **Upload to WordPress**: The generated images, along with their metadata, will be automatically uploaded to your WordPress media library.

This process is simple, automated, and customizable to fit your specific needs.

## How It Works

The workflow consists of several automated steps to ensure seamless image generation and upload:

1. **Generate Image Prompts**: Based on your blog title, the tool creates three detailed prompts for image generation.
2. **Define Workflow Parameters**: These prompts are then passed as parameters to the image generation step.
3. **Generate Images**: The AI model (Stable Diffusion) uses the prompts to create images.
4. **Upload Media to WordPress**: The images are uploaded to your WordPress media library with appropriate metadata (title, description).
5. **Define Workflow Outputs**: The final outputs, including media ID and URLs, are stored and can be used for further processing.

This ensures that each step is connected and automated, making the entire process efficient and easy to manage.

## FAQs

> **Q: How do I enter my blog title?**  
> A: Enter your blog title in the provided field at the start of the process.

> **Q: What kind of images will be generated?**  
> A: The tool generates high-quality, realistic images based on the prompts derived from your blog title.

> **Q: How are the images uploaded to WordPress?**  
> A: The images are automatically uploaded to your WordPress media library along with metadata for easy integration into your blog posts.

> **Q: Can I customize the prompts?**  
> A: Yes, you can customize the prompts to better suit your specific needs.

> **Q: Do I need to fill in any data for WordPress connections?**  
> A: Yes, please fill in the related data at the [credential page](https://app.burstyai.com/user/api-key).

# AI Blog Images Generation & Post to WordPress API

This API workflow generates AI-crafted images based on user inputs and automatically uploads them to WordPress. The process includes creating specific prompts, generating images using an AI model, and handling image uploads with metadata for seamless integration into blog posts.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/6626525bb78aab0001c32426/async_run`

### Method
`POST`

## Description

The workflow facilitates the generation of images using AI models, guided by specific prompts provided by the user. These images are then automatically uploaded to a WordPress blog, complete with appropriate metadata. This service is ideal for bloggers and digital marketers looking to enhance their posts with custom imagery.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `BqNtRV###blog_title` (string, required): The title of the blog post. This title helps guide the thematic focus of the generated images.

### Example JSON Request

```json
{
  "params": {
    "BqNtRV###blog_title": "5 best cities for summer vacation"
  }
}
