# [Free and Automated Website Backlink Research Tool](https://burstyai.com)

## How to Use This Tool

The Website Backlink Research Tool is designed to help you find and analyze backlinks to your competitor's website easily. Here's a step-by-step guide on how to use it:

1. **Enter Competitor's Website URL**: Start by providing the URL of your competitor's website. Make sure it begins with `https://`.
2. **Customize Search Settings**: Adjust the search settings such as the number of search results, country, and language if needed. The default settings work well for most users.
3. **Run the Workflow**: Click on the "Run" button to initiate the backlink research process. The tool will perform a Google search to find backlinks pointing to the specified competitor's website.
4. **Analyze the Results**: The tool will analyze the search results using a language model to categorize the backlinks and identify who posted them. 
5. **View and Export Findings**: The findings will be presented in a structured format, making it easy to analyze and interpret. You can save the output to a sheet on the platform or download it as a CSV file.

## How It Works

This tool leverages a combination of Google search and language model analysis to provide comprehensive backlink research. Here are the detailed workflow steps:

1. **Google SERP Queries**: The tool performs a Google search using specific search terms designed to find backlinks to your competitor's website while excluding results from the competitor's own site.
   - **Input**: Competitor's website URL, number of search results, country, and language settings.
   - **Output**: A list of URLs that link back to the competitor's site.

2. **Query with Language Model**: Each URL is analyzed to determine the category of the website and identify who posted the backlink.
   - **Categorization**: The website is categorized as a directory, public platform, blog, or related business.
   - **Poster Identification**: The tool identifies whether the post was made by the competitor, site owner, influencer, or journalist.

3. **Workflow Outputs**: The final step compiles the analysis into a structured format.
   - **Details**: Snippet, link, title, backlink reason, category, poster, and business website URL are included in the output.
   - **Export Options**: Results can be saved to a sheet or downloaded as a CSV file for further analysis.

## FAQs

> **Q: What information do I need to provide to use this tool?**  
> A: You need to enter the URL of your competitor's website. Optionally, you can adjust search settings like the number of search results, country, and language.

> **Q: Can I customize the search settings?**  
> A: Yes, you can customize the number of search results, the country and language for the search, and other settings as needed.

> **Q: How do I analyze the results?**  
> A: The tool provides a structured output categorizing the backlinks and identifying who posted them. You can save this output to a sheet or download it as a CSV file.

> **Q: Is this tool free to use?**  
> A: Yes, this tool is free to use within the Free subscription plan on BurstyAI.

# Website Backlink Research API

This API workflow researches backlinks to a competitor's website. It performs a Google search for backlinks, analyzes the results using a language model to categorize the backlinks and identify the poster, and formats the findings into a structured output for easy analysis and interpretation.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/6638d64af95dc6000142e77d/async_run`

### Method
`POST`

## Description

This workflow allows users to research backlinks pointing to a competitor's website. It utilizes a Google search to find backlinks, then employs a language model to categorize these links and identify the sources. The output is formatted for easy analysis, aiding in competitive analysis and SEO strategy development.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `KeR0Pf###BURSTYAI_SERP_PAGE_INDEX` (string, optional): The index of the SERP page to retrieve results from. Default is "1".
  - `KeR0Pf###BURSTYAI_SERP_COUNTRY` (string, optional): The country to tailor search results for. Default is "us".
  - `KeR0Pf###BURSTYAI_SERP_LANGUAGE` (string, optional): The language for search results. Default is "en".
  - `KeR0Pf###BURSTYAI_SERP_RESULT_MODE` (string, optional): The output mode for results ("batch" or "individual"). Default is "individual".
  - `KeR0Pf###competitor_website` (string, required): The URL of the competitor's website (starts with https://).
  - `I1cyOE###business_name` (string, required): The name of the competitor's business, used for categorizing and analyzing backlinks.

### Example JSON Request

```json
{
  "params": {
    "KeR0Pf###BURSTYAI_SERP_PAGE_INDEX": "1",
    "KeR0Pf###BURSTYAI_SERP_COUNTRY": "us",
    "KeR0Pf###BURSTYAI_SERP_LANGUAGE": "en",
    "KeR0Pf###BURSTYAI_SERP_RESULT_MODE": "individual",
    "KeR0Pf###competitor_website": "https://www.example.com",
    "I1cyOE###business_name": "Example Business"
  }
}
