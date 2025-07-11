# Maven-Marketing-Campaign-Analysis

## Project Overview
This Power BI dashboard delivers a full-scale, insight-driven analysis of a multinational marketing campaign initiative, focusing on the core metrics that influence customer engagement, campaign success, and revenue performance. It offers a holistic view of campaign outcomes across demographics, countries, sales channels, and product lines—equipping decision-makers with the clarity needed to fine-tune marketing strategies and optimize business impact.

The dashboard begins with a comprehensive campaign overview, showcasing high-level KPIs such as total customers, response rates, average income, and geographic reach. It further dissects customer segmentation, providing detailed insights into age distributions and purchasing patterns—an essential step in refining target audience strategies and improving campaign personalization.

It proceeds to evaluate product-level performance, identifying the top and underperforming product categories, and reveals which offerings are consistently driving the highest sales volume. Coupled with this is a detailed analysis of sales channel effectiveness, comparing in-store, online, and catalog performance to understand which engagement paths yield the best conversion results.

From a geographic lens, the dashboard explores country-level performance, mapping how marketing campaigns and customer responses vary across eight different nations. This cross-country insight helps uncover where campaigns are thriving and where market penetration may need to be re-evaluated.
Overall, this dashboard serves as a strategic intelligence tool, combining performance tracking, behavioral insights, and revenue analysis into a single, interactive platform.
By visualizing performance from multiple angles, it enables stakeholders to uncover untapped opportunities, pinpoint inefficiencies, and make high-impact, data-informed marketing and business decisions.

## Problem Statement
In a competitive business landscape, companies run multiple marketing campaigns across various regions and customer segments, often without fully understanding what drives success or failure. Despite reaching a broad audience, many campaigns underperform due to poor targeting, ineffective channel selection, and limited visibility into customer behavior.

This project seeks to bridge that gap through a data-driven dashboard that transforms raw marketing data into actionable business insights.

To achieve this, the analysis is framed around key business questions across four critical categories:

**1. Customer Demographics & Behavior**

Which age groups make up the majority of our customer base?

How do factors like education and marital status influence engagement?

2. Campaign Performance
Which campaigns generated the highest response rates?

Are certain campaigns more effective in specific countries or demographics?

3. Product & Channel Performance
Which products drive the most revenue?

How do different sales channels perform in terms of conversions and engagement?

4. Geographic & Financial Impact
Which countries contribute most to overall income and campaign success?

Where are marketing efforts underperforming, and why?

By addressing these questions, the project aims to provide business leaders with the clarity needed to refine marketing strategies, maximize ROI, and make smarter, data-informed decisions.

## Data Source
The dataset used for this project was sourced from Maven Analytics, a platform that provides real-world business datasets designed for analytics and BI projects.

This particular dataset simulates a global marketing campaign for a retail company operating in multiple countries. It includes over 2,000 customer records, covering a wide range of variables such as:
- Demographics: Age, education, marital status, and income
- Product purchases: Spending across various product categories
- Sales channels: Web, catalog, in-store, and deals purchases
- Campaign interaction: Response to five different marketing campaigns
- Geographic presence: Country-level customer and income distribution
- Customer service: Complaint history and engagement metrics

## Tools Used
 - Microsoft Power BI (Desktop)

## Data Analysis Process
**1. Data Cleaning using Power Query**

**2. Included some interesting DAX functions**

DAX Measures for calculating KPIs (AVerage Income, Total customers, Total Response etc.)
```DAX
Average Income = SUM(marketing_data[ Income ]) / COUNTROWS(marketing_data)
Total Customer = DISTINCTCOUNT(marketing_data[ID])
Total Response = SUM(marketing_data[Response])
```
**3. Feature Engineering:** Grouped continuous variables like income and age into categories as part of feature engineering to support better demographic segmentation.

















