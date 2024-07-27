# [Free Automated Tool to Transform Top Ranked Pages into Blog Posts](https://burstyai.com)

## How to Use This Tool

1. **Enter Keywords**: Begin by entering the keywords you want to target. These keywords will be used to search for top-ranked pages on Google.
2. **Fetch Top Pages**: The tool will automatically search Google and find the top-ranked pages based on your keywords.
3. **Extract Content**: It will extract key elements like text and images from the top webpage.
4. **Generate Blog Post**: Finally, it will compile these elements into a ready-to-publish blog post.
5. **Customize and Publish**: Review the generated content, make any necessary edits, and publish it on your blog.

## How It Works

1. **Define Workflow Parameters**: Input the search keywords.
2. **Google Search**: The tool searches Google for the top-ranked pages using the specified keywords.
3. **Extract URL and Content**: It extracts the URL and title of the top page and scrapes the content from it.
4. **Aggregate Images**: Images are fetched based on the search and aggregated into an array.
5. **Compile Blog Post**: The extracted text and images are combined to create a comprehensive blog post.
6. **Export Options**: Save the blog post to a sheet or download it as a CSV file for easy publication.

## FAQs

> **Q: How do I enter my search keywords?**  
> **A:** You can enter your search keywords in the designated input field when setting up the workflow.

> **Q: Can I customize the generated blog post?**  
> **A:** Yes, you can review and edit the blog post before publishing it.

> **Q: How are images handled in the blog post?**  
> **A:** The tool fetches and aggregates relevant images based on your keywords, which are then included in the blog post.

> **Q: Can this tool connect to third-party services like WordPress?**  
> **A:** Yes, you can connect it to your WordPress account by entering the required data on the credentials page [here](https://app.burstyai.com/user/api-key), the blog post will post directly to your WordPress website then.

> **Q: Is this tool free to use?**  
> **A:** Yes, it is free to use within the BurstyAI platform's free subscription plan.

# Top Ranked Page to Blog Post API

The "Top Ranked Page to Blog Post" API converts top Google search results into blog posts. This workflow identifies relevant keywords, retrieves the top-ranked webpage, and extracts key content elements such as text and images to create a ready-to-publish blog post, streamlining content creation for digital marketers.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/661393d440216300014edc47/async_run`

### Method
`POST`

## Description

This API transforms top Google search result pages into blog posts by identifying keywords, fetching the top webpage, and extracting key elements like text and images. It is designed to assist digital marketers in quickly generating content from high-ranking sources.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `OAg2aB###search_keywords` (string, required): Keywords used to search for top-ranked web pages on Google.

### Example JSON Request

```json
{
  "params": {
    "OAg2aB###search_keywords": "latest technology trends"
  }
}
