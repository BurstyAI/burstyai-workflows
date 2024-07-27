# [Free Automated LSI Keywords and Entity Extraction Tool](https://burstyai.com)

## How to Use This Tool

1. **Input the Main Keyword**:
   - Enter the primary keyword or phrase representing your niche or topic. This will guide the search to identify top-ranking pages relevant to your topic.
   
2. **Specify the Number of Top Pages**:
   - Define how many of the top-ranked Google search pages you want to analyze. This ensures the extraction focuses on the most relevant and authoritative content.
   
3. **Set the Number of LSI Keywords and Entities**:
   - Indicate how many LSI keywords and entities you want to extract from each page. This helps in gathering comprehensive SEO elements for optimizing your content.
   
4. **Choose the Language**:
   - Select the language for the analysis, aligning with your target audience’s preferences.

## How It Works

1. **Google Search with Seed Keyword**:
   - The tool performs a Google search using the provided keyword, fetching the top 10 search results from the specified country and language settings.

2. **Extract Top N Pages**:
   - From the search results, the tool extracts the URLs of the top N pages. This step focuses on identifying the most authoritative sources for further analysis.

3. **Crawl Page Plain Text**:
   - The tool crawls the content of each extracted page, retrieving the plain text. This ensures that all visible text content is available for keyword and entity extraction.

4. **Extract LSI Keywords and Entities**:
   - Using advanced language models, the tool extracts 100 highly relevant LSI keywords and 50 highly relevant entities from the crawled content. The output is formatted as a JSON object for easy integration.

### FAQs

> **Q: What are LSI keywords?**  
> A: LSI (Latent Semantic Indexing) keywords are terms related to the main keyword that help search engines understand the context and relevance of the content. They improve the SEO and ranking of your page.

> **Q: How does this tool help with SEO?**  
> A: By extracting LSI keywords and entities from top-ranking pages, the tool provides insights into the most relevant terms and concepts. This helps in optimizing your content to match search engine criteria and improve visibility.

> **Q: Can I customize the number of pages and keywords?**  
> A: Yes, you can specify the number of top pages to analyze and the number of LSI keywords and entities to extract. This customization ensures the analysis is tailored to your needs.

> **Q: Is this tool free to use?**  
> A: Yes, the LSI Keywords and Entity Extraction Tool is completely free to use. Enhance your SEO strategy without any cost.

> **Q: What format is the output in?**  
> A: The output is provided in JSON format, making it easy to integrate with other tools or platforms. It includes the extracted LSI keywords, entities, and the target audience for the content.


# LSI Keywords and Entity Extraction API

This API endpoint automates the extraction of LSI keywords and entities from top-ranked Google search pages. The process involves searching keywords, analyzing top URLs, scraping content, and identifying key SEO elements to optimize web presence.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/65fdec982eadbf0001091bf1/async_run`

### Method
`POST`

## Description

This workflow extracts LSI (Latent Semantic Indexing) keywords and entities from top-ranked Google search pages. It searches for the provided keyword, analyzes the top-ranked URLs, scrapes their content, and identifies key SEO elements for optimization.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `iIYNcf###search_keyword` (string, required): The primary keyword or phrase used to perform the Google search.
  - `iIYNcf###top_n_pages` (string, required): The number of top-ranked pages to analyze for extracting LSI keywords and entities.

### Example JSON Request

```json
{
  "params": {
    "iIYNcf###search_keyword": "Artificial Intelligence trends",
    "iIYNcf###top_n_pages": "5"
  }
}
