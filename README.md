# Forage Quantium Data Analytics Job Simulation Project
Overview
This project involved completing 3 tasks as part of Quantium's Data Analytics Virtual Project on Forage. The tasks focused on data preparation, experimentation, uplift testing, and applying analytics for commercial insights.

## Tasks Completed
- Data Preparation and Customer Analytics
- Experimentation and Uplift Testing
- Analytics and Commercial Application

## Dependencies
- Language: Python 3.8
- Packages: pandas, numpy, matplotlib, seaborn, mlxtend, datetime, scipy
## Project Overview and Task Insights 
### Task 1: Data Preparation and Customer Analytics
Files: Quantium_DA_task1(submitted).ipynb, QVI_purchase_behaviour.csv, QVI_transaction_data.xlsx

Data Cleaning: Converted date integers to datetime, removed salsas and outliers.
- Customer Purchase Analysis: Analyzed total sales & no. of customers, grouped by:
  - LIFESTAGE: Identified customer life stages (e.g., families, singles).
  - MEMBERSHIP: Segmented customers by spending habits and product preferences (e.g., Premium, Budget, Mainstream).
- Top 3 sales contributing customer groups analysis: Focused on preferences for chip brand and packet size.

Insights:
- 1. Overall, our stores sell 105 kinds chip products, gaining 1.8million dollars of revenue. Customers spend 7.3 dollars on chips per transaction on average.
- 2. For all customers, the most popular chips' brands are Kettle, Smiths, and Doritos. 175g is the most popular packet size. In general, medium-to-large size chips seems more popular.
- 3. Christmas’ Eve had the peak number of transaction and total sales, indicating that holidays or family gathering events lead to increases of interests in chips.
- 4. Top 3 sales contributing customer segments are Budget Older families, Mainstream Young Singles/Couples, and Mainstream Retirees.
- 5. Factors driving sales:
     - A) Mainstream Young Singles/Couples takes up the largest proportion of customers.
     - B)Mainstream Young & Midage Singles and Couples are more willing to buy more packet of chips on average and pay more per chips, which is indicative of impulse buying behavior.
     - C) Older Families & Young Families buy more chips per customer.

### Task 2: Experimentation and Uplift Testing
Files: Quantium_DA_task2.ipynb, QVI_data.csv
- Trial Stores: Three stores (77, 86, 88) tested new layouts (Feb-Apr 2019).
- Control Stores: Identified control stores using Pearson correlations and magnitude distances.
- Hypothesis Testing: Compared total sales and customer metrics between trial and control stores.
Insights:
- 1. The control stores successful reflect the performance of trial stores, instead of the average of other stores, based on the performance of total sales and number of customers.
- 2. The results for trial stores 77 and 88 during the trial period show a significant difference in at least two of the three trial months but this is not the case for trial store 86.
- 3. Overall, the trial shows a significant increase in sales during trial period.

- Control and Trial Pairs:
  - Store 77 and 233
  - Store 86 and 155
  - Store 88 and 237

Conclusion:
- Store 77: Trial succeed, they are significantly different. The driver of change is from both increases in total sales and number of customers.
- Store 86: The number of customers is significantly higher in all three months, but sales is not. Check trial store’s trial period implementation.
- Store 88: Trial succeed. The driver of change is more from the number of customers than sales.

### Task 3: Analytics and commercial application
Prepared a PowerPoint report summarizing key insights from Tasks 1 and 2 using the Pyramid Principle.

## Limitation & Suggestion
It is suggested that the stores should improve their product naming system or format to avoid statistical bias. such as naming the product name in a format like "Brand & Flavor & Product Category & Weight/Size”.
The reasons are:
- • The original database lack of clarification in product category. It is also not easy to tell if the
product is chips product, cheese product, or salsa product or other kinds just by looking at the
product names. This can lead to significant bias from different kinds of misunderstanding.
- • The brand names and product category in the current product name column are not unique. One
brand has more than one brand names, and chip product has more than one category name. Without further communication with the stores, or fully understanding of products, analyst might generate analysis with bias or just inaccurate.
