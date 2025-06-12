# iFood Campaign Analytics: Brazil’s Hidden Behemoth
![iFood_Hero_Pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/ifood_project_pic.png)

## Executive Summary
**iFood is the leading food delivery platform in Brazil**, surpassing American counterparts like DoorDash and Uber Eats. Founded in 2011, iFood connects restaurants, couriers, and customers through a seamless app experience, offering on-demand food and grocery delivery while **commanding over 80% of Brazil’s market share.** 

The Recency, Frequency, Monetary (RFM) Model is used to group customers by purchasing behavior: Top Customer, Loyal Customer, Promising, At-Risk, and Lost customer segments. The majority of campaign respondents across the marketing campaigns were Loyal Customer (37%) and At Risk (27%) segments. The Loyal Customer segment generated a significant portion of total revenue at 47%. **To maximize return on investment (ROI), the Loyal Customer segment should be prioritized, as it generated an ROI of 3.1 across all campaigns.** Future campaigns should incorporate the top demographic attributes of higher income, absence of family, and older age, which correlate to higher spend.

The following sections will enhance customer profiling and explore ways to personalize marketing campaigns to inform targeting strategies and budget allocation.

Below is the overview page from the Tableau dashboard and more examples are included throughout the report. View the entire interactive [Tableau dashboard](https://public.tableau.com/app/profile/steven.hiek/viz/iFoodCampaignAnalytics/iFoodDashboard).

![Tableau_dashboard_overview_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Executive_summary_dashboard.png)
## Background
The company has data on existing customer demographics, marketing campaigns, and purchasing behavior that have been previously underutilized. This project thoroughly analyzes and synthesizes this data in order to uncover critical insights to improve iFood’s marketing campaigns through maintaining customer retention. The analysis is intended to inform strategic decisions made by key stakeholders in the Marketing and Sales department.

Insights and recommendations are provided on the following key areas:
* **Customer Segmentation**: Evaluation of customer segmentation through Recency, Frequency, and Monetary (RFM) analysis, incorporating Gross Customer Lifetime Value (CLV) and regression analysis based on demographic attributes.
* **Campaign Performance**: An analysis of marketing campaign effectiveness, focusing on total customer spend, Cost per Conversion (CPC), and ROI.
* **Purchasing Behavior**: A review of purchasing behavior patterns across key customer segments, highlighting preferences by product offering, product category, purchase channel, and discount affinity.

The Excel workbook used to inspect, clean, and analyze the data can be found [here](https://github.com/stevenhiek/iFood-Campaign-Analytics/tree/main/Analysis).

## Data Structure & Initial Checks
The dataset includes customer demographics, purchasing behavior, and information from 5 marketing campaigns. It has 2205 total rows with each row corresponding to a unique customer that was randomly selected. There were 184 duplicate rows that were removed, resulting in 2021 unique customer rows within the data. The raw data, prior to cleaning, can be found [here](https://github.com/stevenhiek/iFood-Campaign-Analytics/tree/main/Data).

Prior to beginning the analysis, a variety of checks were conducted for quality control and familiarization with the dataset. The data cleaning and data quality checks can be found in the worksheets, *Data Cleaning* and *Data Quality Checks*, [here](https://github.com/stevenhiek/iFood-Campaign-Analytics/tree/main/Analysis).

## Insights Deep Dive
### Customer Segmentation
* The **majority of campaign respondents across the marketing campaigns were from the Loyal Customer segment (37%),** indicating strong campaign appeal to this segment. Campaign 3 stood out by disproportionately attracting the At-Risk segment (39%), highlighting a potential opportunity to explore effective engagement strategies for this segment.
* While the Top Customer segment holds the highest Gross CLV of $1,303, the **Loyal Customer segment contributes the largest share of total revenue at 42%**. Given strong campaign response by the Loyal Customer segment, there is an opportunity to further capitalize on engagement with this segment.
* Despite Brazil’s strong cultural emphasis on family, regression analysis (R² = 0.71) shows that **higher income, absence of family, and older age are strongly associated with an increase in total customer spend.**

![Customer_segmentation_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Customer_demographics.png)

### Campaign Performance
* Campaign respondents have an **average total spend of $1,023, which is 2.3 times greater than that of non-respondents**, indicating that campaign engagement is strongly associated with higher customer spend.
* Overall performance across campaigns shows the **lowest CPC at $63 within the Loyal Customer segment**, reinforcing its status as a high-value, cost-efficient segment. In contrast, while the Top Customer segment has the highest CLV, its CPC is nearly 3x higher at $179, indicating lower cost-efficiency.
* Campaign 2 underperformed with an ROI of -0.3, indicating a loss on investment. While **Campaign 5 delivered the strongest return at 3.5**, suggesting effective targeting or messaging strategies that should be analyzed and potentially replicated.

![Campaign_performance_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Campaign_performance.png)

### Purchasing Behavior
* Total customer spend on regular products is fairly stable across customer segments, resulting in a **total spend of 94% on regular products and 6% on premium products for campaign respondents.** This indicates limited traction for premium products and presents an opportunity to reassess pricing, positioning, or promotional strategies to boost premium product adoption.
* As integral parts of Brazilian culture, **wine and meat are the most popular products across customer segments**, accounting for 59% and 28% of total purchases, respectively. This reveals an opportunity to deepen engagement through promotions, bundling, or loyalty programs centered around these core products.
* **Physical stores are the most preferred purchase channel at 42% across customer segments,** suggesting a potential desire for immediate gratification or social interaction.

![Purchasing_behavior_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Purchasing_Behavior.png)

## Recommendations
Based on the uncovered insights, the following recommendations have been provided:
* With nearly half (46%) of customers in the Promising and At-Risk segments, **targeted engagement strategies should be prioritized to prevent churn and nurture potential growth.**
* **Target campaigns to the Loyal Customer segment featuring exclusive offers, referral incentives, and cross-sell opportunities** to effectively drive further growth and maximize return on investment, since this high-value segment drives 47% of revenue and maintains a low CPC of $63.
* **Personalize marketing campaigns by leveraging key demographic drivers on customer spend – higher income, absence of family, and older age (R² = 0.71)** – while avoiding the low ROI -0.3) of Campaign 2 and following the success of the high ROI (3.5) of Campaign 5 by optimizing messaging, audience selection, and channel use to reduce CPC and improve conversion.
* Opportunity to capitalize on the 42% customer preference in purchasing through physical stores by **enhancing in-store marketing and visibility with targeted signage, displays, and location-based promotions.**  

## Assumptions and Caveats
Throughout the analysis, multiple assumptions were made to manage the challenges with the data. These assumptions and caveats are noted below:
* Sample data is representative of the iFood’s customer base as a whole. 
* Campaigns costs were the same across campaigns since data does not have campaign costs; campaign cost dummy variable was used to help illustrate cost per campaign conversion. 
* Gross customer lifetime value was used instead of customer lifetime value with profit per customer.
* Used a combined RFM score to create broader segments rather than concatenating recency, frequency, and monetary to create granular classifications.



**Visit my [LinkedIn](https://www.linkedin.com/in/stevenhiek/).**
