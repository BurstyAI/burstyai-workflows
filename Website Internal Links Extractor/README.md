# [Free Automated Website Internal Links Extractor](https://burstyai.com)

## How to Use This Tool

Using the Website Internal Links Extractor is simple and effective. Follow these steps to automate the extraction of internal links from any website:

1. **Define Your Website URL**: Enter the URL of the website from which you want to extract internal links. This URL will be the starting point for the tool to navigate through the site.
2. **Set Parameters**: Specify the depth of scraping and other parameters as needed. You can customize the scraping depth to determine how many levels of links to extract.
3. **Run the Workflow**: Start the extraction process. The tool will automatically scrape the website, extract internal links, and gather relevant data.
4. **View and Download Results**: Once the extraction is complete, you can view the results in a structured format. The data can be downloaded as a CSV file or saved to a sheet in the platform.

## How It Works

The Website Internal Links Extractor uses a series of automated steps to gather and summarize internal links from a specified website. Here’s a detailed breakdown of the workflow:

1. **Parameter Definition**:
   - Input the target website URL and define other scraping parameters.
   - The tool sets up the parameters to ensure it extracts relevant internal links.
  
    ```json
    {
      "website_url": "https://example.com"
    }
    ```

2. **Link Extraction**:
   - The tool uses web scraping technology to navigate through the specified website.
   - It identifies and extracts internal links based on the defined parameters.

3. **Data Summarization**:
   - After extracting the links, the tool summarizes the data.
   - It generates a structured output containing titles, descriptions, and URLs of the internal links.

    ```json
    {
      "title": "Sample Title",
      "description": "Sample description of the link",
      "url": "https://example.com/internal-link"
    }
    ```

4. **Output Generation**:
   - The summarized data is formatted and ready for download.
   - Users can save the output to a sheet or download it as a CSV file for further analysis.

## FAQs

### Q: What is the Website Internal Links Extractor?

A: The Website Internal Links Extractor is a tool that automates the process of extracting internal links from any specified website, summarizing the data into a structured format for easy analysis.

### Q: How can this tool help improve my website?

A: By extracting and analyzing internal links, you can gain insights into your website’s link structure, identify potential SEO improvements, and ensure proper internal linking for better navigation and user experience.

### Q: Is this tool free to use?

# Website Internal Links Extractor API

This API endpoint automates the extraction of internal links from a specified website and summarizes the content. It involves defining the target URL, scraping for links, summarizing the extracted data, and outputting titles, descriptions, and URLs in a structured format.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/65ff4b6627e996000198562d/async_run`

### Method
`POST`

## Description

This workflow extracts internal links from a specified website. It begins with a target URL, navigates the site to find all internal links within the domain, and provides a summary of the extracted data, including titles, descriptions, and URLs.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `CjIz1a###website_url` (string, required): The URL of the website from which to extract internal links. This URL serves as the starting point for the web crawler.

### Example JSON Request

```json
{
  "params": {
    "CjIz1a###website_url": "https://burstyai.com"
  }
}
