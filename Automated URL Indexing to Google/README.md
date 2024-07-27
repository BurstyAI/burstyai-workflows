# [Automated URL Indexing to Google](https://burstyai.com)

## How to Use This Tool

This automated tool fetches your recent WordPress posts and submits their URLs to Google for indexing. Follow these steps to use it effectively:

1. **Set Up Your WordPress Integration**:
   - Configure the tool to fetch posts published within a specific timeframe by setting the "Hours Ago" parameter.
   - Ensure your WordPress site is correctly connected to the BurstyAI platform by configuring it [**Credential**](https://app.burstyai.com/user/api-key) page.

2. **Configure Google API Credentials**:
   - Upload your Google API credentials JSON file to authenticate and allow URL submission to Google. 
   - If you need help obtaining the JSON file, refer to the [**how-to-get-a-google-json-key**](https://help.gsctool.com/features/google-indexing/how-to-get-a-google-json-key).

3. **Run the Workflow**:
   - Execute the workflow through the interactive form. The tool will automatically fetch the latest posts and submit their URLs to Google.
   - You can embed this workflow into your website using an iframe for seamless integration.

4. **Review and Download Results**:
   - Check the results directly on the BurstyAI platform.
   - Download the results as a CSV file for your records.

## How It Works

The Automated URL Indexing to Google workflow operates in two main steps:

1. **Fetch Recent WordPress Posts**:
   - The tool retrieves posts published within the specified timeframe (default is 24 hours).
   - This ensures that only your latest content is considered for indexing.

2. **Submit URLs to Google**:
   - The tool uses your Google API credentials to authenticate the requests.
   - URLs of the fetched posts are submitted to Google for indexing, helping to improve their visibility and search engine ranking quickly.

## FAQs

> **Q: How do I connect my WordPress site to BurstyAI?**  
> A: You can connect your WordPress site by following the integration steps provided in the BurstyAI dashboard under the WordPress section.

> **Q: Where can I get the Google API credentials JSON file?**  
> A: You can get the JSON file from your Google Cloud Platform account. Refer to this [**guide**](https://help.gsctool.com/features/google-indexing/how-to-get-a-google-json-key) for detailed instructions.

> **Q: Can I customize the timeframe for fetching posts?**  
> A: Yes, you can set the "Hours Ago" parameter to specify how far back the tool should fetch posts. 

> **Q: How do I embed the workflow on my website?**  
> A: You can embed the workflow using the iframe embedding code provided in the BurstyAI platform. Simply copy and paste the code into your website’s HTML.

> **Q: How can I save the results of the workflow?**  
> A: You can save the results to a sheet on the BurstyAI platform or download them as a CSV file for further analysis.

# Automated URL Indexing to Google API

This API endpoint fetches recent WordPress posts and submits their URLs to Google for indexing. It automates the process, ensuring your latest content is quickly indexed by Google, improving visibility and search engine ranking.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/660091a89a905a000161f688/async_run`

### Method
`POST`

## Description

This workflow automates the submission of recent WordPress post URLs to Google for indexing. It fetches posts published within a specified time frame and submits them using provided Google API credentials.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `feDQjJ###BURSTYAI_GOOGLE_CREDENTIALS_JSON` (string, required): The JSON file containing Google API credentials necessary for URL submission. Ensure proper configuration and permissions.
  - `LaKolC###BURSTYAI_WORDPRESS_POST_HOURS_AGO` (string, required): The number of hours ago to filter WordPress posts. Only posts published within this time frame will be considered for indexing.

### Example JSON Request

```json
{
  "params": {
    "feDQjJ###BURSTYAI_GOOGLE_CREDENTIALS_JSON": "{\"type\": \"service_account\", ...}",
    "LaKolC###BURSTYAI_WORDPRESS_POST_HOURS_AGO": "24"
  }
}
