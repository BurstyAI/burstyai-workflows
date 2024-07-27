# [Free Keyword Search Intent Analyze Tool](https://burstyai.com)

## How to Use This Tool

Using the Free Keyword Search Intent Analyze Tool is easy and intuitive. Here's a step-by-step guide to help you get started:

1. **Input Keywords**: Start by entering the keywords you want to analyze. These keywords will be used to query Google SERP (Search Engine Results Page) data.
2. **Set Parameters**: Customize your search by selecting the country and language preferences. This will tailor the search results to your specific needs.
3. **Run the Analysis**: Click the 'Run' button to start the workflow. The tool will fetch and analyze the top search results for your keywords.
4. **View Results**: The analysis will display the content type, target audience, and search intent for each keyword. You can download the results as a CSV file or save them to a sheet within the platform.

## How It Works

The Keyword Search Intent Analyze Tool follows a detailed workflow to deliver accurate insights:

1. **Google SERP Queries**: The tool queries Google SERP using the specified keywords. It retrieves the top search results, focusing on various aspects such as articles, products, user-generated content (UGC), and more.
2. **Search Intent Analysis**: The tool uses a sophisticated AI model to analyze the SERP data. It answers key questions:
   - Are the majority of ranking URLs articles, products, or UGC?
   - Who is likely searching for these keywords (beginners, experts, buyers)?
   - What is the search intent behind each keyword?
   - What should a page targeting each keyword include to satisfy the user?
   - How in-depth should content be to satisfy the query?
3. **Target Persona Summary**: Based on the analysis, the tool generates a summary of 2-3 target personas. Each persona includes a page goal and information on how to make the page more helpful for that audience.

## FAQs

> **Q: How do I input keywords for analysis?**  
> A: Simply type your keywords into the 'Search Keywords' field and the tool will use these for the SERP analysis.

> **Q: Can I customize the country and language for my search?**  
> A: Yes, you can select the desired country and language to tailor the search results to your preferences.

> **Q: How do I integrate this tool into my website?**  
> A: You can embed the interactive form UI into any website using an iframe embedding code provided by the tool.

> **Q: Can I save the analysis results?**  
> A: Yes, you can save the results to a sheet within the platform or download them as a CSV file.

# Keyword Search Intent Analyze API

This API endpoint analyzes search intent using Google SERP data. It queries specific keywords and analyzes the results to determine content type, target audience, and search intent.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/6601db5fef613a0001568827/async_run`

### Method
`POST`

## Description

This workflow analyzes search intent based on Google Search Engine Results Pages (SERP) data. It retrieves SERP data for specified keywords, analyzing it to determine the type of content, the intended audience, and the underlying search intent.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `lnZCqr###BURSTYAI_SERP_SEARCH_WORDS` (string, required): Keywords for which to analyze search intent.
  - `lnZCqr###BURSTYAI_SERP_COUNTRY` (string, optional): The country for which the search results should be tailored. Defaults to "us".
  - `lnZCqr###BURSTYAI_SERP_LANGUAGE` (string, optional): The language for the search results. Defaults to "en".

### Example JSON Request

```json
{
  "params": {
    "lnZCqr###BURSTYAI_SERP_SEARCH_WORDS": "machine learning",
    "lnZCqr###BURSTYAI_SERP_COUNTRY": "us",
    "lnZCqr###BURSTYAI_SERP_LANGUAGE": "en"
  }
}
