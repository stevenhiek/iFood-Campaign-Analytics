# iFood Campaign Analytics: Brazil’s Hidden Behemoth
![iFood_Hero_Pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/ifood_project_pic.png)

## Project Background
iFood is the leading food delivery platform in Brazil, surpassing American counterparts like DoorDash and Uber Eats. Founded in 2011, iFood connects restaurants, couriers, and customers through a seamless app experience, offering on-demand food and grocery delivery while commanding over 80% of Brazil’s market share. 

The company has data on existing customer demographics, marketing campaigns, and purchasing behavior that have been previously underutilized. This project thoroughly analyzes and synthesizes this data in order to uncover critical insights to improve iFood’s marketing campaigns through maintaining customer retention. The analysis is intended to inform strategic decisions made by key stakeholders in the Marketing and Sales department.

Insights and recommendations are provided on the following key areas:
* **Customer Segmentation**: Evaluation of customer segmentation through Recency, Frequency, and Monetary (RFM) analysis, incorporating Gross Customer Lifetime Value (CLV) and regression analysis based on demographic attributes.
* **Campaign Performance**: An analysis of marketing campaign effectiveness, focusing on total customer spend among respondents and Cost per Conversion (CPC) across customer segments.
* **Purchasing Behavior**: A review of purchasing behavior patterns across key customer segments, highlighting preferences by product offering, product category, purchase channel, and discount affinity.

The Excel workbook used to inspect, clean, and analyze the data can be found [here](https://github.com/stevenhiek/iFood-Campaign-Analytics/tree/main/Analysis).

## Data Structure & Initial Checks
The dataset includes customer demographics, purchasing behavior, and information from 5 marketing campaigns. It has 2205 total rows with each row corresponding to a unique customer that was randomly selected. There were 184 duplicate rows that were removed, resulting in 2021 unique customer rows within the data. The raw data, prior to cleaning, can be found [here](https://github.com/stevenhiek/iFood-Campaign-Analytics/tree/main/Data).

Prior to beginning the analysis, a variety of checks were conducted for quality control and familiarization with the dataset. The data cleaning and data quality checks can be found in the worksheets, *Data Cleaning* and *Data Quality Checks*, [here](https://github.com/stevenhiek/iFood-Campaign-Analytics/tree/main/Analysis).

## Executive Summary
### Overview of Findings
iFood customer portfolio reveals that 55% of customers fall into low-engagement, At-Risk and Lost customer segments, with the Loyal Customer segment generating a significant portion of total revenue at 42%. The following sections will enhance customer profiling and explore ways to personalize marketing campaigns to inform targeting strategies and budget allocation.

Below is the overview page from the Tableau dashboard and more examples are included throughout the report. View the entire interactive [Tableau dashboard](https://public.tableau.com/app/profile/steven.hiek/viz/iFoodCampaignAnalytics/iFoodDashboard).

![Tableau_dashboard_overview_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Executive_summary_dashboard.png)

## Insights Deep Dive
### Customer Segmentation
* RFM analysis indicates that a **majority of customers fall within the At-Risk (43%) and Lost (12%) segments**, highlighting a significant decline in customer engagement and the need for targeted retention efforts.
* While the Top Customer segment holds the highest Gross CLV of $1,303, the **Loyal Customer segment contributes the largest share of total revenue at 42%**. 
* Despite Brazil’s strong cultural emphasis on family, regression analysis (R² = 0.71) shows that **higher income, absence of family, and older age are strongly associated with an increase in total customer spend.**

![Customer_segmentation_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Customer_demographics.png)

### Campaign Performance
* Campaign respondents have an **average total spend of $1,023, which is 2.3 times greater than that of non-respondents.**
* The **Loyal Customer segment has the highest share of campaign respondents at 37%**, followed by the At-Risk segment at 27%.
* Overall performance across campaigns shows the **lowest CPC at $6.29 within the Loyal Customer segment**, while the Top Customer segment records a significantly higher CPC of $17.86.
* While CPC remained relatively consistent across most campaigns, **Campaign 2 has a sharp increase in CPC at $38.46**, whereas Campaign 4 at the lowest CPC with $6.45.

![Campaign_performance_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Campaign_performance.png)

### Purchasing Behavior
* Total customer spend on regular products is fairly stable across customer segments, resulting in a **total spend of 92% on regular products and 8% on premium products for campaign respondents.**
* **Wine and meat are the most popular products across customer segments**, accounting for 54% and 29% of total purchases, respectively.
* **Physical stores are the most preferred purchase channel at 46% across customer segments,** followed by website purchases at 33%.
* Campaign respondents have a low affinity to discount purchases at 12% across customer segments while the **discount purchases accounts for 21% in non-respondents.**

![Purchasing_behavior_pic](https://github.com/stevenhiek/iFood-Campaign-Analytics/blob/main/Charts%2C%20Graphs%2C%20and%20Other/Purchasing_Behavior.png)

## Recommendations
Based on the uncovered insights, the following recommendations have been provided:
* With 55% of customers in the At-Risk and Lost segments, there is an **opportunity to diversify the customer portfolio by reactivating lapsed users and expanding engagement across underrepresented segments** through re-engagement campaigns, loyalty perks, or win-back offers.
* **Target campaigns to the Loyal Customer segment featuring exclusive offers, referral incentives, and cross-sell opportunities** to effectively drive further growth and maximize return on investment, since this high-value segment drives 42% of revenue and maintains a low CPC of $6.29.
* **Personalize marketing campaigns by leveraging key demographic drivers on customer spend – higher income, absence of family, and older age (R² = 0.71)** – while avoiding the high CPC of $38.46 in Campaign 2 by optimizing messaging, audience selection, and channel use to reduce CPC and improve conversion. 
* Opportunity to capitalize on the 46% customer preference in purchasing through physical stores by **enhancing in-store marketing and visibility with targeted signage, displays, and location-based promotions.**  

## Assumptions and Caveats
Throughout the analysis, multiple assumptions were made to manage the challenges with the data. These assumptions and caveats are noted below:
* Sample data is representative of the iFood’s customer base as a whole. 
* Campaigns costs were the same across campaigns since data does not have campaign costs; campaign cost dummy variable was used to help illustrate cost per campaign conversion. 
* Gross customer lifetime value was used instead of customer lifetime value with profit per customer.
* Used a combined RFM score to create broader segments rather than concatenating recency, frequency, and monetary to create granular classifications.



**Visit my [LinkedIn](https://www.linkedin.com/in/stevenhiek/).**
