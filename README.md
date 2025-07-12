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
- Which age groups make up the majority of our customer base?
- How do factors like education and marital status influence engagement?

**2. Campaign Performance**
- Which campaigns generated the highest response rates?
- Are certain campaigns more effective in specific countries or demographics?

**3. Product & Channel Performance**
- Which products drive the most revenue?
- How do different sales channels perform in terms of conversions and engagement?

**4. Geographic & Financial Impact**
- Which countries contribute most to overall income and campaign success?
- Where are marketing efforts underperforming, and why?

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

## Insight Deep Dive

This dashboard presents a comprehensive analysis of a multi-channel retail business with physical store, catalog, and online presence. The analysis evaluates marketing campaign performance, customer engagement, product sales, and income distribution across various countries and sales channels. Insights are grouped by business functions to support decision-making

#### 1. Customer Demographics & Behavior
**Age Group Dominance:** Over 60% of customers fall within the 1960–1980 birth range, identifying mid-aged adults as the primary market segment. These customers likely have stable income and high purchasing power.

**Average Income:** The typical customer earns around $52K, with a significant concentration in the $50K–100K range, making them ideal targets for premium product and loyalty campaigns.

#### 2. Campaign Performance & Response
**Low Overall Conversion:** Out of 2,000 customers, only 334 responded, giving a response rate of 16.7%, highlighting room for campaign optimization.

**Best-Performing Campaigns:** Campaign 4 (25%) and Campaigns 3 & 5 (24.4%) outperformed others, suggesting stronger personalization or timing strategies.

**Country-Specific Effectiveness:** Spain showed the highest campaign impact, while countries like Mexico and the USA had low or no responses—implying poor market penetration or engagement.

#### 3. Product Performance Analysis
**Top Revenue Drivers:** Wines were the dominant product category, generating over 50% of total product sales.

Meat Products followed at 27.5%, while other categories like Fruits and Sweet Products lagged.

**Sales Seasonality:** Sales peaked in August and October, possibly aligning with seasonal promotions or campaigns. These periods can be leveraged in future planning.

**Product Popularity by Country:** Despite regional differences, Wines consistently outperformed across most countries. India, however, showed a higher affinity for Meat and Gold Products.

#### 4. Country-Level Insights
**Top Market: Spain**

Spain accounted for the highest engagement (54K) and revenue ($56M) but also logged the most customer complaints, signaling a service or delivery gap.

**Emerging Markets:** Countries like Canada, Australia, and India show moderate revenue with low complaints—indicating room for growth through strategic investment.

**Underperforming Regions:** Mexico and the USA showed zero to low revenue, making them candidates for market re-evaluation or targeted entry campaigns.

#### 5. Channel Effectiveness
**Store Purchases Dominant in Use:** Although Store Purchases saw the highest traffic (13K), they did not correlate with proportionate revenue—highlighting conversion inefficiency.

**Catalog and Deals Channels:** These channels contributed to revenue but were underutilized compared to their performance, offering opportunities for promotion.

**Country-wise Channel Behavior:** Channel effectiveness varied by country. For instance, Web Visits and Store Purchases dominated in Europe, while Catalog and Deals performed better in countries like Mexico and India.

#### 6. Income Distribution & Trend
**Income by Channel:** Highest income came from Store and Web Purchase channels within the $50K–100K range. There’s an opportunity to upsell higher-value products in these streams.

**Income by Year:** Revenue was consistently strong between 2013 and 2014, peaking at $15.9M. Slight drops around mid-2013 and early 2014 may reflect seasonal slumps or campaign fatigue.

**Education Impact on Income:** Customers with a Graduation degree contributed over $59M, far ahead of others—highlighting education as a strong revenue predictor.

#### 7. Customer Complaint Patterns
**Complaints Concentrated in Spain (14 cases):** While Spain had high revenue and engagement, it also led in complaints—implying potential issues in product fulfillment, communication, or logistics.

**Low Complaint Regions:** Countries like Australia, Mexico, and USA recorded no complaints, which may either reflect lower engagement or stronger satisfaction.

## Business Recommendations
#### 1. Optimize Campaign Strategy
- **Replicate Top Campaigns:** Leverage insights from high-performing campaigns (Campaigns 4, 3, and 5) to develop future outreach. Analyze timing, messaging, and segmentation used.
- **Re-target Low-Response Segments:** Re-evaluate campaigns with low conversion, like Campaign 2, and test different audience groups or delivery channels.
- **Improve Personalization:** Tailor campaigns to align with age, income, and education profiles—especially for the 1960–1980 age group and graduate-level customers.

#### 2. Focus on High-Value Markets
- **Double Down on Spain & Saudi Arabia:** These markets show strong engagement and revenue—invest in strengthening logistics and customer experience there.
- **Unlock Potential in Canada & Australia:** With decent performance and low complaints, they are ideal for marketing expansion and strategic promotions.
- **Reassess Mexico & USA Strategy:** These markets show poor performance—evaluate market demand, product fit, and awareness before allocating further resources.

#### 3. Channel Optimization
- **Improve Conversion in Physical Stores:** Store visits are high, but revenue isn’t matching. Consider improving customer journey, in-store promotions, and sales staff training.
- **Scale Underutilized Channels:** Channels like Catalog Purchases and Deals drive revenue with low engagement—invest in awareness and access.
- **Leverage Regional Channel Preferences:** Tailor channel mix based on region—for instance, boost Catalog in Mexico and Deals in Germany.

#### 4. Product Strategy Enhancement
- **Expand High-Margin Products:** Wines and Meat Products are top revenue contributors—consider bundling, upselling, or premium variations of these categories.
- **Re-evaluate Low-Performing Products:** Fruits and Sweet Products contribute little to revenue—either reposition them or cut back on marketing investment.

#### 5. Address Customer Experience Gaps
- **Investigate High Complaint Regions:** Spain, despite its revenue, has the most complaints. Review fulfillment, customer service, and delivery processes.
- **Monitor Silent Markets:** Countries with zero complaints (e.g., Mexico, USA) may have low engagement rather than full satisfaction—investigate customer feedback loops.

#### 6. Revenue Growth Tactics
- **Capitalize on Sales Peaks:** August and October have strong sales—consider replicating the promotional strategy or expanding campaigns during these months.
- **Target High-Income Segments:** Customers earning $50K–$100K drive revenue. Customize offers, loyalty perks, and premium product messaging for them.

##  Conclusion
This project provides a comprehensive analysis of a multi-channel retail business by evaluating customer demographics, campaign effectiveness, product performance, and income distribution across regions and channels. Through the interactive Power BI dashboard, key trends and gaps were uncovered—such as underutilized sales channels, high-potential markets, top-performing campaigns, and revenue-driving products.

The insights generated enable data-driven decision-making across marketing, sales, and operations. From refining campaign strategies to optimizing product focus and improving customer engagement, this analysis equips stakeholders with a clear understanding of what’s working, what isn’t, and where to focus future efforts.

Overall, the dashboard serves as a powerful business intelligence tool, offering actionable insights that can enhance campaign ROI, boost customer satisfaction, and support sustainable growth across markets.

## Author
[Benard Gabriel] - Data Analyst 

















