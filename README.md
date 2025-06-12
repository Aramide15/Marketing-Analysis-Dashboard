## 2023/2024 Loan App Marketing Analysis Report

### Project overview
This is an interactive Power BI dashboard designed for comprehensive marketing performance analysis. The dashboard helps stakeholders gain insights into customer behavior, campaign effectiveness, and key marketing metrics to support data-driven decision-making.

### Table of Content
1. [Data source](#data-source)
2. [Tools and Technologies](#tools-and-technologies)
3. [Data cleaning and preparation](#data-cleaning-and-preparation)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-(eda))
5. [Data Analysis](#data-analysis)
6. [Results/Findings](#results/findings)
- [Insight 1](#insight-1)
- [Strategic business recommendations](#strategic-business-recommendations)
- [Insight 2](#insight-1)
- [Strategic business recommendations](#strategic-business-recommendations)
7. [Limitations](#limitations)
8. [References](#references)

### Data Source
Marketing data: This is the primary dataset used for this analysis "Marketing data.xlsx". This contains detailed information about loan type, gender of each visitors on the app, amount borrowed, campaign type, etc.

### Tools and Technologies
- Microsoft word: Used for taking note and documenting my findings
- Excel : Used for data cleaning [Download Here](https://www.microsoft.com)
- Powerbi : Used for data analysis and creating dashboard for reporting purpose


### Data cleaning and preparation
In this phase, the steps below were taken to prepare and clean the data for analysis:
1. Load the dataset into excel
2. Insert filter into the table of dataset to be able to view and understand the values in the table of dataset
3. Used condtional formmatting to create a categorical column in the table of dataset
4. Removed Null value

### Exploratory Data Analysis (EDA)
EDA also called Exploratory Data Analysis is done after data cleaning and data prepartion has be completed. This is used to answer key business questions to draw insights from. These are questions to answered with this dataset:

1. Total customers/Visitors
2. Total Revenue generated
3. Total amount borrowed
4. Average revenue generated
5. Revenue generated per campaign_Name
6. Revenuue generated per gender
7. Monthlty revenue generated
8. Which campaign generated the highest revenue within the year?
9. Which age_group came into the app often and the highest revenue generated per age_group?
10. The conversion rate of each campaign per revenue.

### Data Analysis
These are some codes and formular used in this analysis
1. Excel
```Excel
=IFS(D2:D2001<=30,"Youth",D2:D2001<50,"Middleage",D2:D2001<=60,"Elderly")
```
2. Powerbi Query
```Powerbi
Signup_month = 'Cleaned data'[SignupDate].[Month]
```
```Powerbi
Average_revenue = AVERAGE('Cleaned data'[RevenueGenerated])
```
```powerbi
Total Conversion rate = SUM('Cleaned data'[ConversionRate])
```

### Results/Findings 

#### Insight 1
##### Total Revenue: 
A combined total of ₦302.73 million was generated across all campaigns from 2023 to 2024. 
- In 2023, revenue amounted to ₦215.83 million, with the LoanBlitz campaign contributing the 
highest at ₦45 million. 
- In 2024, revenue totaled ₦86.90 million, led by the Back-to-School campaign, which generated 
₦22 million. 
##### Total Customers Acquired: 
A total of 2,000 customers were acquired during the reporting period. 
- 1,438 customers were acquired in 2023, 
- 562 customers were acquired in 2024. 
##### Total Amount Borrowed: 
The total amount borrowed across all campaigns from 2023 to 2024 was approximately ₦2 billion. 
- In 2023, borrowing reached ₦1 billion, 
- While in 2024, ₦425 million was borrowed. 

#### Strategic business recommendations 
1. Reinforce High-Performing Campaigns 
- Recommendation: Consider relaunching or expanding the LoanBlitz and Back-to-School 
campaigns. 
- Rationale: These campaigns generated the highest revenues in their respective years. Optimizing 
their timing, reach, and targeting could increase impact and ROI. 
2. Investigate 2024 Decline and Refocus Marketing Strategy 
- Recommendation: Conduct a root cause analysis for the significant drop in revenue, customer 
acquisition, and loan disbursement in 2024. 
- Rationale: Understanding market changes, customer behavior, or internal execution gaps will 
guide adjustments in messaging, channels, or campaign structures. 
3. Target Customer Segments with High Borrowing Potential 
- Recommendation: Use insights from 2023’s higher borrowing volume to identify customer 
profiles or regions with strong borrowing demand and prioritize them in future campaigns. 
- Rationale: Tailoring products and campaigns to these segments can drive both customer growth 
and loan uptake. 
4. Optimize Campaign Timing and Budget Allocation 
- Recommendation: Use historical data to time campaigns for peak borrowing periods and 
allocate more budget toward proven performers. 
- Rationale: This ensures resources are invested in campaigns that align with customer demand 
and seasonal patterns. 
5. Implement Performance-Based Campaign Tracking
- Recommendation: Establish clear KPIs for each campaign (e.g., revenue per customer, cost per 
acquisition, loan-to-customer ratio) and track them in real-time. 
- Rationale: This allows for early intervention and continuous optimization during campaign 
cycles.

#### Insight 2
#### Conversion Rate Overview 
A total conversion rate of 950.76 was recorded across all campaigns between 2023 and 2024. 
- Kano maintained the highest overall conversion rate across the two years. 
- In 2023, Abuja led with a conversion rate of 141.75. 
- In 2024, Ibadan recorded the highest conversion rate at 57.05. 
#### Revenue Generated per Product 
The Walletonly product was the top revenue-generating product, contributing a total of ₦82.27 million 
from 2023 to 2024. 
- It remained the most utilized product on the platform in both years. 
#### Conversion Rate by Campaign 
- In 2023, the LoanBlitz campaign achieved the highest conversion rate among all campaigns. 
- In 2024, the Back-to-School campaign led in terms of conversion performance.

#### Strategic business recommendations 
1. Double Down on High-Converting Regions 
- Recommendation: Allocate more marketing resources to Kano, Abuja, and Ibadan, which 
consistently showed strong conversion rates. 
- Rationale: These regions have demonstrated higher responsiveness to campaigns and can serve 
as benchmarks or pilot zones for future rollouts. 
2. Optimize and Scale Walletonly Product 
- Recommendation: Continue to prioritize the Walletonly product in promotional efforts, while 
exploring opportunities to enhance features, bundles, or cross-sell options. 
- Rationale: With ₦82.27 million in revenue, it is the top-performing product and has shown 
sustained popularity across both years. 
3. Replicate Successful Campaign Structures 
- Recommendation: Analyze the strategies used in the LoanBlitz (2023) and Back-to-School 
(2024) campaigns and use those insights to structure future campaigns (e.g., messaging, timing, 
targeting). 
- Rationale: These campaigns delivered the highest conversion rates in their respective years and 
offer a proven model for success. 
4. Introduce Region-Specific Campaigns 
- Recommendation: Design campaigns tailored to high-performing locations like Abuja and 
Ibadan, based on their specific customer behavior and needs. 
- Rationale: Regional customization can improve engagement and conversion rates by aligning 
offers with local preferences. 
5. Strengthen Conversion Rate Monitoring & Analysis 
-Recommendation: Set up a real-time dashboard to track conversion rates per region, product, 
and campaign, and establish thresholds for intervention. 
- Rationale: Monitoring conversion performance closely enables agile responses and continuous
campaign optimization.

### Limitations
1. Lack of a Data Dictionary: 
The absence of a data dictionary made it challenging to accurately interpret the purpose of each 
column within the dataset. Including a dedicated reference sheet with column definitions, data 
types, and business logic would have significantly improved data understanding and analysis 
accuracy. 
2. Inconsistent Column Naming: 
Some column names lacked standardization or used abbreviations that were unclear, leading to 
additional time spent validating assumptions with available context clues. For example the 
Ischurned column value could have been in yes/no value. 
3. Missing or Null Values: 
Certain fields contained null or missing values, especially in campaignName and transaction 
records. These were treated as unknowns during analysis, but a clear rule on how to handle such 
gaps would be beneficial for future reporting. 
4. Data Format Issues: 
In a few cases, numerical fields were formatted as text, which required cleaning and reformatting 
before analysis could proceed.

### References
1. Linkedin
2. Google chrome browser
