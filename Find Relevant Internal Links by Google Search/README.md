# [Free Automated Tool to Find Relevant Internal Links by Google Search](https://burstyai.com)

## How to Use This Tool

Our **Free Automated Tool to Find Relevant Internal Links by Google Search** is designed to help you enhance your website's SEO and user experience effortlessly. This tool leverages Google Search to identify the most relevant internal links on your website based on a given blog title and keyword.

1. **Input your Website URL:** Start by entering the URL of your website where the search will be conducted.
2. **Enter the Blog Title:** Provide the title of the blog post for which you want to find relevant internal links.
3. **Set the Number of Links:** Specify how many internal links you want the tool to find and return.

Simply click on the "Run Workflow" button, and our tool will analyze the search results to find the best matches for your blog post, enhancing your content's SEO.

## How It Works

This tool operates through a series of automated steps to ensure the most relevant internal links are identified:

1. **Google SERP Queries:** The tool initiates a search on Google using the format `site:your_website blog_title`, restricting the search to your website and using the blog title as the keyword.
2. **Query with LLM:** Our tool processes the Google SERP results with a Large Language Model (LLM), analyzing each result to identify the most relevant internal links.
3. **Return Results:** The tool returns the top relevant internal links in a structured format, including the link, title, and a snippet.

This seamless process ensures that you get the best internal links to boost your content's SEO without any manual effort.

## FAQs

> **Q: How do I customize the number of internal links to find?**  
> A: You can set the desired number of internal links in the "Amount of Internal Links" field before running the workflow.

> **Q: Can I use this tool for multiple blog posts?**  
> A: Yes, you can run the workflow multiple times with different blog titles to find relevant internal links for each post.

> **Q: What if the tool doesn't find any relevant internal links?**  
> A: If no relevant links are found, the tool will return an empty result. Ensure your blog title and keywords are specific and accurate.

> **Q: How can I integrate this tool with my website?**  
> A: You can embed the interactive form UI into your website using an iframe embedding code, allowing you to integrate the workflow seamlessly.

# Find Relevant Internal Links by Google Search API

This API workflow identifies the most relevant internal links on your website using Google Search. It analyzes search results based on a given blog title and keyword, providing the best matches to enhance your content's SEO and user experience.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/6643bb9a25d4b70001c61517/async_run`

### Method
`POST`

## Description

The workflow uses Google Search to find the most relevant internal links for a specified blog post title. By leveraging search data, it helps improve SEO and user engagement by linking to relevant content within your website.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `TGt3Qs###website_url` (string, required): The URL of your website where the search will be focused. This restricts the search to your domain.
  - `TGt3Qs###blog_title` (string, required): The title of the blog post for which you want to find relevant internal links. This serves as the keyword for the search.
  - `TGt3Qs###amount_of_internal_links` (string, required): The number of most relevant internal links to find and return. For example, "1" returns the top relevant link, "2" returns the top two, etc.

### Example JSON Request

```json
{
  "params": {
    "TGt3Qs###website_url": "google.com/blog",
    "TGt3Qs###blog_title": "Guide to Effective Content Marketing",
    "TGt3Qs###amount_of_internal_links": "2"
  }
}

