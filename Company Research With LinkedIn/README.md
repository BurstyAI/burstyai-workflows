# [Free and Automated Company Research with LinkedIn](https://burstyai.com)

## How to Use This Tool

This automated workflow is designed to extract detailed company data from LinkedIn, making it perfect for personalized outreach. Here’s how you can use it:

1. **Access the Workflow**: Start by opening the [BurstyAI platform](https://app.burstyai.com).
2. **Input the LinkedIn URL**: Enter the LinkedIn URL of the target company in the provided field.
3. **Run the Workflow**: Click the "Run" button to initiate the extraction process.
4. **Review the Results**: The workflow will extract and display company details including name, description, industries, employee range, HQ location, tagline, and funding info.
5. **Get a Summary**: You will also receive a 120-word summary tailored to your product or service for personalized outreach.
6. **Save or Download**: Save the results to a sheet in BurstyAI or download them as a CSV file.

## How It Works

This customizable workflow consists of several steps to ensure accurate and comprehensive data extraction:

1. **Input Collection**: The workflow begins by collecting the target company's LinkedIn URL from the user.
2. **LinkedIn API Integration**: The URL is used to fetch detailed company information through LinkedIn's API.
3. **Data Extraction**: Extracted data includes company name, description, industries, specialties, employee range, HQ location, tagline, and funding info.
4. **Summary Generation**: An AI model generates a personalized 120-word summary based on the company data and your product/service description.
5. **Output Delivery**: The final data, including the summary, is presented in an interactive form UI, which can be embedded on any website using an iframe.

## FAQs

> **Q: How do I input the LinkedIn URL of the company?**
> 
> A: Enter the LinkedIn URL in the "Target Company LinkedIn URL" field provided in the workflow interface.

> **Q: Can I customize the extracted data format?**
> 
> A: Yes, you can customize the workflow parameters using the no-code drag-and-drop builder in BurstyAI.

> **Q: How can I integrate this workflow into my website?**
> 
> A: Use the iframe embedding code provided by BurstyAI to embed the workflow form on your website.

> **Q: Where is the extracted data saved?**
> 
> A: The data can be saved to a sheet within BurstyAI or downloaded as a CSV file.

# Company Research With LinkedIn API

This API workflow extracts detailed company data from LinkedIn, including information such as the company's name, description, industries, employee range, HQ location, tagline, and funding information. It also generates a 120-word summary tailored to your product or service for personalized outreach.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/663b81a8baf9a500013b25c5/async_run`

### Method
`POST`

## Description

The workflow collects and analyzes company data from LinkedIn, providing a comprehensive profile that includes key business details and a concise summary. This information is ideal for marketers and sales professionals looking to personalize their outreach strategies.

## Request Body

The request body must be a JSON object containing the following field:

- `params`: Object containing the required parameter.
  - `OkIy9G###company_linkedin_url` (string, required): The LinkedIn URL of the target company.

### Example JSON Request

```json
{
  "params": {
    "OkIy9G###company_linkedin_url": "https://www.linkedin.com/company/example"
  }
}
