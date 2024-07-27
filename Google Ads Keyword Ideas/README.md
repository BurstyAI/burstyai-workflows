# [Free Automated Google Ads Keyword Ideas Tool](https://burstyai.com)

## How to Use This Tool

To start using the **Google Ads Keyword Ideas Tool**, follow these simple steps:

1. **Access the Tool**: Go to the [BurstyAI platform](https://app.burstyai.com).
2. **Enter Details**: Input your desired **keywords** or a **website URL**. You can use both for better results.
3. **Set Parameters**: Choose your **location IDs** and **language ID** to tailor the suggestions to your target audience.
4. **Run the Tool**: Click the run button to fetch keyword suggestions, including metrics like average monthly searches and competition levels.
5. **View Results**: Check the keyword ideas and metrics on the results page.
6. **Download Data**: Save the results to a sheet in the platform or download them as a CSV file for further analysis.

You can also embed this tool on your website using an iframe embedding code provided by BurstyAI.

## How It Works

The **Google Ads Keyword Ideas Tool** leverages Google's Ads API to provide you with relevant keyword suggestions. Here's a step-by-step breakdown of the workflow:

1. **Input Seed Keyword/URL**: Start by providing a seed keyword, a website URL, or both.
2. **API Request**: The tool sends a request to the Google Ads API with the provided inputs.
3. **Fetch Data**: The API retrieves keyword suggestions along with metrics like average monthly searches, competition levels, and trends.
4. **Data Processing**: The tool processes the data and maps it to predefined workflow parameters such as keyword, average monthly searches, competition value, etc.
5. **Display Results**: The processed data is displayed in an interactive form on the platform.
6. **Save or Download**: Users can save the results to a sheet or download them as a CSV file for further use.

### FAQs

> **Q: Do I need to sign up to use this tool?**  
> A: Yes, you need to create a free account on BurstyAI to access and use the tool.

> **Q: Can I customize the keyword suggestions for different locations and languages?**  
> A: Yes, you can input specific location IDs and language IDs to tailor the keyword suggestions.

> **Q: How can I embed this tool on my website?**  
> A: You can embed the tool using the iframe embedding code provided by BurstyAI.

> **Q: Where can I find the location and language IDs?**  
> A: Location IDs can be found [here](https://developers.google.com/google-ads/api/data/geotargets) and language IDs [here](https://developers.google.com/google-ads/api/data/codes-formats#languages).

# Google Ads Keyword Ideas API

This API uses Google's Ads API to fetch keyword suggestions, providing metrics like average monthly searches and competition levels. It supports customization for specific geographic and language settings, and can be used with a seed keyword, a website URL, or both.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/663551c8baf9a500013b254e/async_run`

### Method
`POST`

## Description

The workflow retrieves keyword ideas from Google's Ads API, tailored to specific geographic locations and languages. It generates keyword suggestions based on a provided seed keyword or website URL, offering valuable insights for keyword research and advertising strategies.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `egoYUP###BURSTYAI_GOOGLEADS_LOCATION_IDS` (string, optional): Space-separated IDs for geographic targeting, e.g., 2840 for the US. A list of location IDs can be found [here](https://developers.google.com/google-ads/api/data/geotargets).
  - `egoYUP###BURSTYAI_GOOGLEADS_LANGUAGE_ID` (string, required): ID representing the language for generating keyword ideas, default is 1000 for English. Language IDs can be found [here](https://developers.google.com/google-ads/api/data/codes-formats#languages).
  - `egoYUP###BURSTYAI_GOOGLEADS_KEYWORD_TEXTS` (string, optional): Space-separated keywords for generating ideas. Either this or `BURSTYAI_GOOGLEADS_PAGE_URL` must be provided.
  - `egoYUP###BURSTYAI_GOOGLEADS_PAGE_URL` (string, optional): A reference website URL to extract keyword ideas from. Either this or `BURSTYAI_GOOGLEADS_KEYWORD_TEXTS` must be provided.

### Example JSON Request

```json
{
  "params": {
    "egoYUP###BURSTYAI_GOOGLEADS_LOCATION_IDS": "2840",
    "egoYUP###BURSTYAI_GOOGLEADS_LANGUAGE_ID": "1000",
    "egoYUP###BURSTYAI_GOOGLEADS_KEYWORD_TEXTS": "ai automation",
    "egoYUP###BURSTYAI_GOOGLEADS_PAGE_URL": ""
  }
}
