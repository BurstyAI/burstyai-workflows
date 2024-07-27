# [Free Automated Company Research Tool](https://burstyai.com)

## How to Use This Tool

This free and automated tool helps you gather detailed information about any company just by using its website. Here's how you can use it:

1. **Input the Website URL:** Start by entering the company's website URL in the provided field. Make sure it starts with 'https'.
2. **Run the Workflow:** Click on the 'Run' button to start the process. The tool will scrape the company's website to collect data.
3. **Get Your Results:** Once the scraping is complete, you will get a structured summary that includes the company's name, description, niches, objectives, audience, pain points, value propositions, tone, contacts, social links, and an opportunity summary for personalized outreach.
4. **Download or Save:** You can download the results as a CSV file or save them to a sheet in the platform for future use.

## How It Works

The tool works in a few simple steps:

1. **Scrape the Home Page:** It starts by scraping the company's home page to gather text and links.
2. **Analyze the Data:** Using advanced language models, it analyzes the gathered data to extract important business information.
3. **Compile the Summary:** The tool compiles the data into a structured summary that includes essential details about the company.
4. **Provide Output:** Finally, it outputs the information, which can be downloaded or saved for your records.

The tool uses no-code drag-and-drop features, making it customizable and easy to use for anyone, even those without technical skills. Plus, you can embed the interactive form UI into any website using an iframe embedding code.

## FAQs

> **Q: Do I need any technical skills to use this tool?**    
> A: No, this tool is designed to be user-friendly and requires no technical skills. You can easily use it with a simple drag-and-drop interface.

> **Q: Can I customize the workflow?**    
> A: Yes, the workflow can be customized to fit your needs using the no-code builder. You can adjust parameters and settings as needed.

> **Q: How can I integrate this tool with my website?**    
> A: You can embed the interactive form UI into your website using the provided iframe embedding code. This allows you to integrate the workflow seamlessly.

> **Q: What output formats are available?**    
> A: You can save the output to a sheet on the platform or download it as a CSV file.

Start using the Free Automated Company Research Tool today to simplify your research process and enhance your outreach efforts!

# Company Research With Its Website API

This API workflow scrapes and analyzes a company's website to gather detailed business information. It provides a structured summary of the company's name, description, niches, objectives, audience, pain points, value propositions, tone, contacts, social links, and a concise opportunity summary for personalized outreach.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/663b63baf95dc6000142e79c/async_run`

### Method
`POST`

## Description

This workflow scrapes a company's website to collect and analyze information. It generates a structured summary covering various aspects of the business, including name, description, niches, objectives, target audience, pain points, value propositions, tone, contact details, social media links, and potential opportunities for personalized outreach.

## Request Body

The request body must be a JSON object containing the following field:

- `params`: Object containing the required parameter.
- `OkIy9G###business_website` (string, required): The URL of the target business website, starting with 'https', e.g., 'https://google.com'.

### Example JSON Request

```json
{
  "params": {
    "OkIy9G###business_website": "https://example.com"
  }
}
