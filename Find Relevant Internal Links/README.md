# [Free Automated Tool for Finding Relevant Internal Links](https://burstyai.com)

## How to Use This Tool

Our **Free Automated Tool for Finding Relevant Internal Links** helps you identify the best internal links from your website based on a specified keyword. This tool is designed to enhance your content's SEO and improve user experience by finding the most relevant internal links for your blog posts. 

To use the tool:

1. **Input the Blog Title**: Enter the title of your blog post. This will serve as the keyword to search for relevant links.
2. **Specify the Number of Links**: Indicate how many internal links you want to find. You can choose to get the most relevant link or multiple top links.
3. **Run the Workflow**: Execute the workflow to analyze your data and return the best matches.

### Features
- **No-Code Customization**: Customize your search parameters without any coding skills.
- **Interactive Form**: Use the built-in form to execute the workflow and get results instantly.
- **Easy Integration**: Embed the form on your website using an iframe to seamlessly integrate the workflow.

## How It Works

The **Find Relevant Internal Links** tool uses advanced algorithms to search and retrieve the best matches for your specified keyword from your website’s data entries. Here’s a step-by-step breakdown of the process:

1. **Input Data**: The workflow starts by taking your input parameters (blog title and number of links).
2. **Data Splitting**: It splits the data into manageable chunks for efficient processing.
3. **Query Execution**: The tool uses a language model to query the data and find the most relevant entries.
4. **Data Aggregation**: It aggregates the results and selects the top matches based on your specified number of links.
5. **Output Results**: Finally, it returns the most relevant internal links, including the URL, title, and description of each link.

### Benefits
- **Improves SEO**: Enhances your content’s search engine optimization by linking to relevant internal pages.
- **Boosts User Engagement**: Helps users find more related content on your site, increasing page views and engagement.
- **Saves Time**: Automates the process of finding internal links, saving you time and effort.

## FAQs

> **Q: How many internal links can I find with this tool?**  
> 
> A: You can specify the number of links you want to find. The tool can return the most relevant link or multiple top links based on your input.

> **Q: Do I need any technical skills to use this tool?**  
> 
> A: No, this tool is designed for non-technical users. You can easily customize and use it without any coding knowledge.

> **Q: Can I integrate this tool into my website?**  
> 
> A: Yes, you can embed the interactive form on your website using an iframe code provided by BurstyAI.

> **Q: Where can I save the output results?**  
> 
> A: You can save the results to a sheet within the platform or download them as a CSV file.

> **Q: How do I connect this tool to my WordPress?**  
> 
> A: You can fill in the necessary data on the credentials page [here](https://app.burstyai.com/user/api-key).

# Find Relevant Internal Links API

This API workflow identifies the most relevant internal links from your website based on a specified keyword. It analyzes data entries to find and return the best matches, helping to enhance your content's SEO and user experience.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/66436d0c0c01970001f2d88a/async_run`

### Method
`POST`

## Description

The workflow analyzes your website's data to find the most relevant internal links for a given blog post title. By providing relevant internal links, it helps improve SEO and user navigation on your site.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `bz0nkE###BURSTYAI_CHUNK_SIZE` (string, required): The number of items each chunk should contain. For example, a value of "1" will process items individually.
  - `TGt3Qs###blog_title` (string, required): The title of the blog post for which you want to find relevant internal links. This title serves as the keyword to identify relevant links.
  - `TGt3Qs###amount_of_internal_links` (string, required): The number of most relevant internal links to find and return. For example, "1" returns the top relevant link, "2" returns the top two, and so on.

### Example JSON Request

```json
{
  "params": {
    "bz0nkE###BURSTYAI_CHUNK_SIZE": "50",
    "TGt3Qs###blog_title": "Guide to Effective Content Marketing",
    "TGt3Qs###amount_of_internal_links": "2"
  }
}
