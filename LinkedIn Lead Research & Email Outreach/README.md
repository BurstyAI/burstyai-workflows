# [Free and Automated LinkedIn Lead Research & Email Outreach](https://burstyai.com)

## How to Use This Tool

Using the LinkedIn Lead Research & Email Outreach tool is simple and effective. This automated workflow helps you research LinkedIn leads and send personalized emails to them. Here’s how you can use it:

1. **Input LinkedIn URL**: Enter the LinkedIn profile URL of the lead you want to research.
2. **Fill in Sender Information**: Provide your name, job role, and a summary of your business.
3. **Customize Outreach Objectives**: Define your goals for reaching out, such as setting up a meeting or introducing a product.
4. **Run the Workflow**: Click the start button to fetch and analyze the LinkedIn data, generate personalized insights, and create a tailored email.

This tool automates your lead generation process, making it easier to engage potential leads effectively.

## How It Works

The LinkedIn Lead Research & Email Outreach tool operates through a series of automated steps:

1. **Fetch LinkedIn Data**: The workflow starts by gathering information from the LinkedIn profile URL you provided.
2. **Analyze and Generate Insights**: It analyzes the lead's profile to extract personalized insights that can be used for engagement.
3. **Create Tailored Emails**: Based on the insights, the tool generates a customized email to ensure effective communication.
4. **Save and Download**: You can save the output to a sheet on the platform or download it as a CSV file for further use.

With its no-code drag-and-drop builder, you can customize the workflow to fit your needs, making lead generation and email outreach a breeze.

## FAQs

> **Q: Do I need a LinkedIn account to use this tool?**  
> 
> A: Yes, you need access to LinkedIn to fetch lead data.

> **Q: Can I integrate this workflow into my website?**  
> 
> A: Absolutely! Use the iframe embedding code to integrate the workflow into any website.

> **Q: How do I set up my email server for outreach?**  
> 
> A: Fill in the required data on the credential page [here](https://app.burstyai.com/user/api-key).

> **Q: Can I customize the email template?**  
> 
> A: Yes, the tool allows you to customize the email template to match your outreach objectives.

> **Q: Is this tool free to use?**  
> 
> A: Yes, it is free within the BurstyAI free subscription plan.

# LinkedIn Lead Research & Email Outreach API

This API workflow performs LinkedIn lead research and email outreach. It retrieves a lead's LinkedIn data, analyzes it for personalized insights, and generates a tailored email for outreach. The workflow automates the process, ensuring effective and engaging communication with potential leads.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/664352f9e3d8f80001200c56/async_run`

### Method
`POST`

## Description

The workflow automates the process of researching LinkedIn leads and crafting personalized emails. By analyzing the lead's LinkedIn profile, it gathers insights and generates an email tailored to the outreach objective, which can include scheduling meetings, introducing products, or exploring collaborations.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `2gbpFd###OkIy9G###lead_linkedin_url` (string, required): The URL of the LinkedIn profile for the lead you want to research and engage with.
  - `QtWEfq###1DWkUe###outreach_objective` (string, required): The main goal or objective of the outreach, such as scheduling a meeting, introducing a product, or discussing a potential collaboration.

### Example JSON Request

```json
{
  "params": {
    "2gbpFd###OkIy9G###lead_linkedin_url": "https://www.linkedin.com/in/williamhgates/",
    "QtWEfq###1DWkUe###outreach_objective": "Discuss potential collaboration opportunities"
  }
}
