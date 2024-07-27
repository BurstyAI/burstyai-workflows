# [Free Keyword Ideas by Google Search Auto-completion](https://burstyai.com)

## How to Use This Tool

Getting started with the Keyword Ideas by Google Search Auto-completion tool is easy and efficient. Follow these simple steps to generate valuable keyword ideas:

1. **Sign Up or Log In**: Access the BurstyAI platform and sign up for a free account or log in if you already have one.
2. **Navigate to the Tool**: Find the "Keyword Ideas by Google Search Auto-completion" tool under the SEO category.
3. **Enter Your Search Query**: Input your desired search keywords and select the language for the search.
4. **Run the Workflow**: Click the run button to start the workflow. The tool will use Google's Suggestqueries API to simulate auto-complete suggestions based on your input.
5. **Review the Results**: Once the process is complete, you can view the generated keyword ideas. These can be saved to a sheet in the platform or downloaded as a CSV file for further use.

## How It Works

The Keyword Ideas by Google Search Auto-completion tool automates the process of generating keyword ideas through the following steps:

1. **Call Google Suggestqueries API**: The tool initiates a request to Google's Suggestqueries API, using your specified keywords and language to simulate a search query.
2. **Fetch Auto-complete Suggestions**: The API returns a list of auto-complete suggestions related to your input keywords.
3. **Convert XML to JSON**: The raw data from the API, in XML format, is converted to JSON using a large language model (LLM). This ensures the data is structured and easy to read.
4. **Output Results**: The JSON data is then presented to you in a user-friendly format. You can download the results or integrate them into your website using an iframe embedding code.

## FAQs

> **Q: Can I customize the workflow?**  
> A: Yes, the workflow can be personalized to suit your needs. You can adjust the search keywords, language, and other parameters without any coding.

> **Q: How do I integrate the workflow into my website?**  
> A: You can embed the workflow using an iframe code provided by BurstyAI. This allows you to integrate the keyword generation process directly into your website.

> **Q: Is there a limit to the number of keyword ideas I can generate?**  
> A: There is no limit within the free subscription plan. You can run the tool as many times as needed to generate a comprehensive list of keyword ideas.

# Keyword Ideas By Google Search Auto-completion API

This API uses Google's Suggestqueries API to generate keyword ideas by simulating auto-complete suggestions based on a user-specified search query. It helps in identifying potential keywords for content creation and SEO strategies.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/662fdc6c127126000108f047/async_run`

### Method
`POST`

## Description

The workflow leverages Google's auto-complete feature to suggest keyword ideas based on an initial search query. It simulates user inputs and captures auto-complete suggestions, which are useful for generating keyword lists for SEO and content development.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `WvJUah###PROXY123_PROXY_COUNTRY` (string, optional): Proxy country code, such as US, CN, or UK. Default is "US".
  - `WvJUah###PAGE_DOWNLOAD_TILL` (string, required): Specifies how far to load the page; typically set to "load".
  - `WvJUah###search_lang` (string, required): Search language code, such as en or cn. Default is "en".
  - `WvJUah###search_keywords` (string, required): The initial search keyword used to trigger auto-completion suggestions.

### Example JSON Request

```json
{
  "params": {
    "WvJUah###PROXY123_PROXY_COUNTRY": "US",
    "WvJUah###PAGE_DOWNLOAD_TILL": "load",
    "WvJUah###search_lang": "en",
    "WvJUah###search_keywords": "ai automation"
  }
}
