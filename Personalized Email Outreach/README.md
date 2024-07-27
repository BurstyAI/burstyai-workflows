# [Free Personalized Email Outreach Tool - Automated & Customizable](https://burstyai.com)

## How to Use This Tool

1. **Sender and Prospect Information**: Sender information cloud be obtained by Onboarding workflow, Prospect data could be obtained by 'Lead Research With LinkedIn' workflow.
2. **Input Your Information**: Provide your details like your name, position, and relevant background information. This helps in personalizing the email.
3. **Enter Your Business Summary**: Add a brief summary of your business to introduce it in the email.
4. **Add Prospect Information**: Input details about the prospect, such as their name, position, and company. 
5. **Include Engaging Points**: Gather data points from the prospect's latest LinkedIn posts or profile. This will be used to craft a personalized opening line.
6. **Define Outreach Objective**: Clearly state the objective of your outreach. This helps tailor the email to achieve your specific goals.

By following these steps, you can create a personalized cold email that is engaging, relevant, and likely to get a positive response.

## How It Works

1. **Define Workflow Parameters**:
   - Enter your sender information and business summary.
   - Provide details about the prospect and engaging points from their LinkedIn profile.
   - State the outreach objective.

2. **Create Opening Line**:
   - The tool generates a casual, non-salesy opening line based on the prospect's data points and your business information.

3. **Query with LLM**:
   - The tool uses advanced AI to write the complete email. It combines the opening line with the value proposition and outreach objective to create a personalized email.

4. **Save and Download**:
   - Once the email is generated, you can save it to a sheet in the platform or download it as a CSV file.

### FAQs

- **Q: How do I connect to my email server?**
  - A: Fill in the related data on the credential page here: [API Key](https://app.burstyai.com/user/api-key).

- **Q: Can I customize the workflow parameters?**
  - A: Yes, you can customize the parameters using the no-code drag-drop builder.

- **Q: How do I integrate the workflow into my website?**
  - A: Use the iframe embedding code provided in the interactive form UI to embed the workflow into any website.

- **Q: Is there a cost to use this tool?**
  - A: No, this tool is free within the Free subscription plan in BurstyAI.

- **Q: Can I download the generated emails?**
  - A: Yes, you can save the output to a sheet in the platform or download it as a CSV file.

# Personalized Email Outreach API

This API workflow creates a personalized cold email for outreach, generating an engaging opening line and a complete email based on the sender's information, business summary, and the prospect's LinkedIn data points. The aim is to ensure the email is relevant, personal, and likely to elicit a positive response.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/663f40e20ce0ef0001569b51/async_run`

### Method
`POST`

## Description

The workflow generates personalized cold emails by leveraging details about the sender and the prospect, including information gathered from LinkedIn. It creates a relevant and engaging email, helping to improve the chances of a positive response.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `1DWkUe###sender_information` (string, required): Details about the sender, including name, position, and relevant background information.
  - `1DWkUe###sender_business_summary` (string, required): A brief summary of the sender's business, highlighting its value proposition.
  - `1DWkUe###prospect_information` (string, required): Details about the prospect, such as name, position, company, and any other relevant information.
  - `1DWkUe###prospect_engaging_points` (string, required): Engaging data points about the prospect, derived from their LinkedIn posts or profile, to personalize the outreach.
  - `1DWkUe###outreach_objective` (string, required): The goal of the outreach, guiding the purpose and desired outcome of the email.

### Example JSON Request

```json
{
  "params": {
    "1DWkUe###sender_information": "Jane Doe, Sales Manager",
    "1DWkUe###sender_business_summary": "XYZ Corp provides innovative tech solutions to streamline business processes.",
    "1DWkUe###prospect_information": "John Smith, CTO at Tech Innovations Inc.",
    "1DWkUe###prospect_engaging_points": "Noticed you recently spoke about AI integration in your product line.",
    "1DWkUe###outreach_objective": "Introduce our AI solutions and explore potential collaboration."
  }
}

