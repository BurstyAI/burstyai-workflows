# Free Automated Topical Authority Map & Blog Plan

## How to Use This Tool

1. **Enter Your Topic Keyword**: Start by providing the main keyword or phrase that represents the niche or topic you want to explore. This will guide the creation of categories and blog content plans.
2. **Specify the Number of Categories**: Define how many unique categories your niche should be divided into. Each category will cover a distinct aspect of the overall topic.
3. **Set the Number of Blog Articles per Category**: Decide how many blog articles should be planned for each category to ensure thorough exploration of each topic.
4. **Select Your Language**: Choose the language for generating categories and blog plans, ensuring it aligns with your target audience's preferences.

## How It Works

1. **Category Creation**: Using the provided keyword, the tool utilizes advanced language models to generate a JSON array of unique sub-categories. Each category is crafted to cover different aspects of the niche without any overlap.
2. **Blog Article Planning**: For each generated category, the tool creates a detailed plan for several unique blog articles. Each article is designed to cover a specific aspect of the category, ensuring comprehensive coverage.
3. **SEO Optimization**: Both categories and blog articles are crafted with SEO in mind, including optimized titles, descriptions, and keywords to improve search engine ranking and attract the right audience.

### FAQs

> **Q: What is a topical authority map?**  
> A: A topical authority map is a structured outline that divides a niche into unique categories, each covering different aspects of the topic, to establish authority in that niche.

> **Q: How does this tool help with SEO?**  
> A: By creating well-defined categories and comprehensive article plans, the tool ensures your content covers all aspects of a topic, improving search engine visibility and authority.

> **Q: Can I customize the number of categories and articles?**  
> A: Yes, you can specify the number of categories and the number of articles per category to tailor the plan to your needs.

> **Q: Is this tool free to use?**  
> A: Yes, the Topical Authority Map & Blog Plan tool is free to use.

> **Q: What languages are supported?**  
> A: The tool supports multiple languages. You can select your preferred language to ensure the content aligns with your audience's preferences.


# Topical Authority Map & Blog Plan API

This API endpoint facilitates the creation of SEO-optimized blog article plans by dividing a given niche into unique categories and generating several articles for each category.

## Base URL

`https://app.burstyai.com/burstyai/aiflows`

## Endpoint

### URL
`/65e1cd00141fdc000195cb88/async_run`

### Method
`POST`

## Description

Creates a blog article plan by dividing a specified niche into unique categories and generating several articles for each category, ensuring all aspects of the topic are covered without repetition.

## Request Body

The request body must be a JSON object containing the following fields:

- `params`: Object containing the required parameters.
  - `5FzC4P###topic_keyword` (string, required): The main keyword or phrase representing the niche or topic to explore.
  - `5FzC4P###amount_of_category` (string, required): The number of unique categories into which the main topic should be divided.
  - `5FzC4P###amount_of_sub_category` (string, required): The number of blog articles planned for each category.
  - `5FzC4P###language` (string, required): The language in which the categories and blog plans should be generated.

### Example JSON Request

```json
{
  "params": {
    "5FzC4P###topic_keyword": "Artificial Intelligence",
    "5FzC4P###amount_of_category": "10",
    "5FzC4P###amount_of_sub_category": "5",
    "5FzC4P###language": "english"
  }
}
