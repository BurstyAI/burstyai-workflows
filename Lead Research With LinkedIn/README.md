# [Free and Automated Lead Research with LinkedIn](https://burstyai.com)

## How to Use This Tool

To use the **Lead Research with LinkedIn** workflow, follow these steps:

1. **Enter LinkedIn URL**: Start by inputting the LinkedIn profile URL of the lead you want to research. This is the only input needed to fetch detailed profile information and recent posts from LinkedIn.
2. **Run the Workflow**: Execute the workflow to automatically fetch and analyze the lead's profile and posts.
3. **View Insights**: Once the workflow is complete, view the personalized data points and insights generated. These insights can help you craft effective cold outreach messages.
4. **Download Results**: You can save the output to a sheet within BurstyAI or download it as a CSV file for further use.

## How It Works

The **Lead Research with LinkedIn** workflow operates through several automated steps:

1. **Fetch LinkedIn Profile**: The workflow fetches the lead's LinkedIn profile details, including their current job title, company, and other relevant information.
2. **Get Recent Posts**: It then retrieves the lead's recent LinkedIn posts.
3. **Aggregate Data**: The retrieved posts are aggregated to extract meaningful data points.
4. **Analyze with AI**: Using AI, the workflow analyzes the profile and posts to generate personalized insights.
5. **Generate Insights**: The final step provides you with detailed data points and insights that can be used to personalize your outreach efforts.

## FAQs

> **Q: What do I need to start using this workflow?**  
> A: You only need the LinkedIn profile URL of the lead you wish to research.

> **Q: Can I customize the workflow parameters?**  
> A: Yes, you can customize the workflow parameters using the no-code drag-and-drop builder.

> **Q: How can I integrate this workflow into my website?**  
> A: You can embed the interactive form UI of this workflow into your website using an iframe embedding code.

> **Q: What output formats are available?**  
> A: The output can be saved to a sheet on the platform or downloaded as a CSV file.

# Lead Research With LinkedIn API

This API workflow fetches and analyzes a lead's LinkedIn profile and recent posts, generating personalized data points and insights for effective cold outreach. It is designed to help marketers and sales professionals gather comprehensive information for personalized communication.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/663ddad1f95dc6000142e7dc/async_run`

### Method
`POST`

## Description

The workflow retrieves detailed information from a lead's LinkedIn profile, including personal details, professional background, and recent activities. It provides insights and personalized data points that can enhance the effectiveness of cold outreach efforts.

## Request Body

The request body must be a JSON object containing the following field:

- `params`: Object containing the required parameter.
  - `OkIy9G###lead_linkedin_url` (string, required): The LinkedIn profile URL of the lead to be researched.

### Example JSON Request

```json
{
  "params": {
    "OkIy9G###lead_linkedin_url": "https://www.linkedin.com/in/williamhgates/"
  }
}

