# Superstore: Profitability Analysis
**Author**: Michel Asselin

**Tools**: Python

**Modules**: pandas, matplotlib, seaborn, numpy. These modules were used for data cleaning, visualization, and statistical analysis.

**Source**: Martin, Michael (October 27, 2022). Sample - Superstore Sales (Excel).xls. Tableau from Salesforce. Retrieved from: https://community.tableau.com/s/question/0D54T00000CWeX8SAL/sample-superstore-sales-excelxls

## Project Overview
This project analyzes the **key drivers of profitability** using the Sample Superstore dataset, a retail dataset originally provided by [Tableau](https://community.tableau.com/s/question/0D54T00000CWeX8SAL/sample-superstore-sales-excelxls) and available on [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final/data?select=Sample+-+Superstore.csv).

The objective is to: 
- Analyze sales and profitability trends from 2014 to 2017.
- Identify the most and least profitable product categories and sub-categories.
- Assess regional and customer segment performance.
- Quantify the impact of discounts and shipping modes on profit margins.
- Translate findings into actionable data-driven recommendations to improve business strategies.

The analysis covers the complete data analytics workflow, from data preparation and visualization to data-driven business recommendations.  

This project was developed in Python (Google Colab environment). The notebook can be run end-to-end using the included dataset (_Sample - Superstore.csv_ found in [this branch](https://github.com/MichelAsselin/data-analysis-portfolio/blob/Superstore-Sales-%26-Profit-Analysis/Sample%20-%20Superstore.csv)). It runs without external setup beyond uploading the CSV.

## Business Questions
**Overall Performance**
- How have sales and profit margin evolved over time?
- Which product categories and sub-categories drive the most profit?
  
**Regional and Segment Insights**
- Which regions and states generate the most revenue and profit?
- Are there regional differences in discount usage?
- Which customer segments are the most valuable?
  
**Profitability Drivers**
- Do discounts negatively affect profit margins?
- What is the relationship between sales volume and profit margin?

**Operational Factors**
- Does the shipping mode affect profitability or delivery efficiency?
- What overall trends can guide better pricing, discounting, and logistics decisions?

## Dataset Information
**Size**: 9,994 sales records

**Main columns**: Order Date, Ship Date, Ship Mode, Segment, State, Region, Category, Sub-Category, Product Name, Sales, Quantity, Discount, Profit

## Workflow
### 1. Data Preparation
- Loaded and cleaned dataset (duplicates removed, data types corrected).
- Created new features such as Profit Margin (%), Sales-Weighted Profit Margin (%), Delivery Time, and Sales-Weighted Discount (%).
- Verified data quality and consistency.

### 2. Exploratory Data Analysis (EDA) & Visualization
For each question, visuals created with matplotlib and seaborn are provided, each accompanied by a business interpretation explaining why the pattern matters.

- _Correlation Heatmap_: Discount has a strong negative correlation (−0.86) with Profit Margin.
<img width="763" height="633" alt="image" src="https://github.com/user-attachments/assets/53879f18-a746-45d8-bc47-39d602375bfa" />

- _Time-Series Analysis_: Sales grew steadily from 2014 to 2017, while margins remained volatile.
<img width="780" height="588" alt="image" src="https://github.com/user-attachments/assets/c08ac815-66c1-47db-870e-60e693304a9b" />

- _Category & Sub-Category Analysis_: Technology and Office Supplies drive profit, while Furniture underperforms.
<img width="780" height="580" alt="image" src="https://github.com/user-attachments/assets/ee6dc246-951e-4ae7-9ce5-2d0af9c78c68" />

- _Regional & State Insights_: West and East regions are most profitable, but Central and South regions do not perform as well.
<img width="730" height="559" alt="image" src="https://github.com/user-attachments/assets/1b440da6-7682-4bea-9bbd-c9fc8e965c6f" />

- _Customer Segments_: Consumer segment contributes the most to overall profit.
<img width="730" height="559" alt="image" src="https://github.com/user-attachments/assets/9d4503d1-2677-4f64-8280-967658a95cde" />

- _Discount Analysis_: Profit margins turn negative once discounts exceed 25–30 %.
<img width="776" height="580" alt="image" src="https://github.com/user-attachments/assets/7233262a-88bc-42d7-bcb6-344c04923a78" />

- _Shipping Mode_: First-Class shipping achieves the highest profit margin, and Standard Class is the least efficient.
<img width="1180" height="490" alt="image" src="https://github.com/user-attachments/assets/be5b0560-e799-45e6-b1bf-04061c4b13c2" />

### 3. Business Insights & Recommendations
1. Discounts are the primary cause of profit loss. Limiting discounts to 25%-30% and implementing category-specific discount limits could reduce profit losses.
2. Furniture has high sales but poor profitability due to steep discounts. Reassess pricing and product strategy, and focus on Furniture items that sell at a loss  to improve profitability.
3. Reinforce strategies for successful and highly profitable sub-categories, such as Copiers, Phones, Accessories, and Papers.
4. Central and South regions lag in profit despite comparable sales to the West and East regions. Use the latter as benchmarks when developing operational improvements.
5. The Consumer segment is the most profitable customer segment. Maintain their engagement through loyalty programs.
6. Improve profitability in Corporate and Home Office segments by reducing discounts and focusing on products with higher profit margins.
7. First Class and Same Day shipping modes provide fast delivery while maintaining healthy profit margins.

## Business Impact
Implementing these recommendations could:
- Increase total profit by reducing unnecessary discounts.
- Improve regional performance through targeted pricing strategies.
- Strengthen long-term profitability without reducing sales volume.

Overall, this analysis provides insights into how discounting and pricing optimization can significantly improve Superstore's profitability. 
