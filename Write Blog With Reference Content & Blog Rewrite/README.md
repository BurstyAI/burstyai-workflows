# [Free Automated Blog Content Creation & SEO Optimization Tool](https://burstyai.com)

## How to Use This Tool

1. **Input Blog Title and Reference Content**
   - Start by entering your blog title and the reference content you want to use.
2. **Generate Summaries and Outlines**
   - The tool will summarize your reference content and create a structured blog outline.
3. **Create Detailed HTML Content**
   - It will generate detailed HTML content for each section of your blog.
4. **Select and Integrate Media**
   - Choose relevant images and videos to enhance your blog post.
5. **Publish to WordPress**
   - Finally, publish your SEO-optimized blog post directly to WordPress.

## How It Works

1. **Summarize Reference Content**
   - The tool takes your input and summarizes the reference content into a structured format.
2. **Create Blog Article Outline**
   - It generates a detailed outline based on your reference content and blog title.
3. **Write Blog Section Content**
   - Each section of the blog is written in HTML, using a clear and engaging language.
4. **Aggregate Data**
   - The content is aggregated and prepared for publishing.
5. **Generate AI Images**
   - The tool generates AI-based image prompts relevant to your blog content.
6. **Review and Merge Media**
   - Images and videos are reviewed and integrated into the blog outline.
7. **Publish to WordPress**
   - The final blog post, complete with SEO metadata, is published to your WordPress site.

## FAQs

> **Q:** How do I start using it, it seems need complex input?
> **A:** This workflow is intended to be used with other workflow which generates inputs for this one.

> **Q:** How do I input my blog title and reference content?
> **A:** You can input these details in the designated fields when you start using the tool.

> **Q:** Can I customize the blog outline and content?
> **A:** Yes, you can customize everything using the no-code drag-drop builder.

> **Q:** How are images and videos added to the blog?
> **A:** The tool selects and integrates relevant images and videos based on your input.

> **Q:** How is the content optimized for SEO?
> **A:** The tool generates SEO metadata and ensures the content is structured with SEO best practices.

> **Q:** Do I need to provide credentials for WordPress publishing?
> **A:** Yes, you will need to fill in your WordPress credentials on the credential page [here](https://app.burstyai.com/user/api-key).

# Write Blog With Reference Content & Blog Rewrite API

This API endpoint automates the creation, optimization, and publishing of blog content. It uses a provided blog title and reference content to generate summaries, outlines, and detailed HTML content, integrates media, and publishes to WordPress with SEO metadata.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/66019fc1ef613a0001568815/async_run`

### Method
`POST`

## Description

Automates the process of creating and optimizing blog content. The workflow includes generating summaries and outlines from a given blog title and reference content, creating detailed HTML content, integrating image and video media, and publishing the content to WordPress with SEO metadata for enhanced visibility and ranking.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `dJUBnI###blog_title` (string, required): The title of the blog post.
  - `dJUBnI###reference_content` (string, required): Content used as a source for generating the new blog post.
  - `dJUBnI###image_resources` (string, required): List of image URLs and their alt texts to be included in the blog post.
  - `dJUBnI###video_resources` (string, required): List of YouTube video URLs to be included in the blog post.

### Example JSON Request

```json
{
  "params": {
    "dJUBnI###blog_title": "Understanding AI in Modern Technology",
    "dJUBnI###reference_content": "AI technology is evolving rapidly...",
    "dJUBnI###image_resources": "['https://example.com/image1.jpg', 'Alt text for image1']",
    "dJUBnI###video_resources": "['https://youtube.com/watch?v=example']"
  }
}
