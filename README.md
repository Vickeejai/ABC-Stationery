# Sales-Report

## Table of Content
[Project Overview](project_overview)

[Data Source](data_source)

### Project Overview

A B C Stationery, a company that deal on the buying and selling of stationeries across the western region of Nigeria has noticed a decline in profit trend and has requested the Data Analysis Team to look at the company’s performance as at year 2013 and 2014. After analyzing the datasets, this report shows the conclusion that A B C Stationary keeps investing in segments that are not producing profits like the Midmarket and Channel Partners across all states. Further insights are shown in this report to gain deeper understanding of the companys performance.

### Data Source _Cargo_

Sales data: The primary dataset used for this analysis is [Football/Soccer Datasets](https://www.kaggle.com/datasets/dissfya/atp-tennis-2013-2023) file.

![](https://github.com/Vickeejai/Sales-Report/blob/main/Screenshot%20(10).png)

### Tools

- Power BI - Data Analysis, DAX Expressions, Creating Reports
  - [Download_here](https://microsoft.com)
 
- PowerPoint - Report Presentation
  - [Download_here](https://microsoft.com)

### Data Cleaning/Preparation

In the initial data preparation phase, we pperformed the following tasks:
1. Data Loading and Inspection
2. Data Cleaning and Formatting using the Power Query Editor

### Exploratory Data Analysis
EDA involved exploring the Office Supply dataset to answer the following questions:

1. Calculate
  - Gross Sales
  - Discount (use the discount rate)
  - Revenue
  - Profit before Tax
  - Profit Margin
  - Tax on Profit (tax rate 5%)
  - Profit after Tax
2. Create a report overview for:
  - Segment
  - State
  - Product
3. Produce a report on all products sold between January and December 2014, showing number of sales, sales proportions and financial performance. This analysis should determine if there is growth or decline on any of the product lines.
4. Compare 2013 Q4 and 2014 Q4 figures to highlight year on year results. Reproduce the report at higher levels such as Product category and State.
5. What key products are the drivers of performance?
6. If we would like to discontinue any product sub due to poor outcomes, what would this be?
7. What product do we pay the highest tax on?
  -  Overall
  - For each state
  - For each segment

### Data Analysis
```Gross Sales = financials3[Units Sold]*financials3[Sale Price]```

```Discount = financials3[Discount Rate]*financials3[Gross Sales]```

```Revenue = financials3[Gross Sales]-financials3[Discount]```

```Profit Before Tax = financials3[Revenue]-financials3[Manufacture Cost]```

```Profit Margin = [Total Profit]/[Total Revenue]```

```Tax on Profit = 0.05*financials3[Profit Before Tax]```

```Profit after Tax = financials3[Profit Before Tax]-financials3[Tax]```

```Sales Proportion = financials3[Manufacture Cost]/financials3[Units Sold]*100```

### Results
2. The report for segmaent, state and product is shown below:

![Screenshot 2024-06-08 172032](https://github.com/Vickeejai/Sales-Report/assets/133552578/40a5ab02-3e77-4c0d-90a8-c056142d5a63)

This visuals shows that Midmarket and Channel Partners made huge losses while small Business made the highest amount of profit in the Segment overview.
Based on State overview, high manufacturing cost in producing products, high revenue was generated but no significant profit gotten.
The production of Staplers and Notepads should be suspended because of the losses made, thereby generating little or no profit in th Product Overview.

3. Report on all products sold between January and December 2014, showing number of sales, sales proportions, financial performance, and if there is growth or decline on any of the product lines.

![Screenshot 2024-06-08 174335](https://github.com/Vickeejai/Sales-Report/assets/133552578/46689d96-99ba-4a45-869d-0d9c64f749f9)

![Screenshot 2024-06-08 174953](https://github.com/Vickeejai/Sales-Report/assets/133552578/8a51151c-9b35-4957-a40b-9d00f0c209a6)























