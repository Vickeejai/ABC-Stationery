# **Financial Analysis Report for ABC Stationery**

---

## **Table of Content**

[Project Overview](project_overview)

[Data Source](data_source)

[Tools](tools)

[Data Cleaning](data_cleaning)

[Exploratory Data Analysis](exploratory_data_analysis)

[Data Analysis](data_analysis)

[Results](results)

[Prescriptive Analysis](prescriptive_analysis)


### **Project Overview**

A B C Stationery, a company that deal on the buying and selling of stationeries across the western region of Nigeria has noticed a decline in profit trend and has requested the Data Analysis Team to look at the company’s performance as at year 2013 and 2014. After analyzing the datasets, this report shows the conclusion that A B C Stationary keeps investing in segments that are not producing profits like the Midmarket and Channel Partners across all states. Further insights are shown in this report to gain deeper understanding of the companys performance.

---

### **Data Source**

Sales data: The primary dataset used for this analysis is [Football/Soccer Datasets](https://www.kaggle.com/datasets/dissfya/atp-tennis-2013-2023) file.

![](https://github.com/Vickeejai/Sales-Report/blob/main/Screenshot%20(10).png)

### **Tools**

- Power BI - Data Analysis, DAX Expressions, Creating Reports
  - [Download_here](https://microsoft.com)
 
- PowerPoint - Report Presentation
  - [Download_here](https://microsoft.com)

### **Data Cleaning**

In the initial data preparation phase, we pperformed the following tasks:
1. Data Loading and Inspection
2. Data Cleaning and Formatting using the Power Query Editor

### **Exploratory Data Analysis**
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

### **Data Analysis**
```Gross Sales = financials3[Units Sold]*financials3[Sale Price]```

```Discount = financials3[Discount Rate]*financials3[Gross Sales]```

```Revenue = financials3[Gross Sales]-financials3[Discount]```

```Profit Before Tax = financials3[Revenue]-financials3[Manufacture Cost]```

```Profit Margin = [Total Profit]/[Total Revenue]```

```Tax on Profit = 0.05*financials3[Profit Before Tax]```

```Profit after Tax = financials3[Profit Before Tax]-financials3[Tax]```

```Sales Proportion = financials3[Manufacture Cost]/financials3[Units Sold]*100```

### **Results**
2. The report for segmaent, state and product is shown below:

![Screenshot 2024-06-08 172032](https://github.com/Vickeejai/Sales-Report/assets/133552578/40a5ab02-3e77-4c0d-90a8-c056142d5a63)

This visuals shows that Midmarket and Channel Partners made huge losses while small Business made the highest amount of profit in the Segment overview.
Based on State overview, high manufacturing cost in producing products, high revenue was generated but no significant profit gotten.
The production of Staplers and Notepads should be suspended because of the losses made, thereby generating little or no profit in th Product Overview.

3. Report on all products sold between January and December 2014, showing number of sales, sales proportions, financial performance, and if there is growth or decline on any of the product lines.

**A4 PAPAER:**
A growth for the last quarter of the year for all parameters.

A B C Stationery experienced their highest Sales Proportion and highest Number of Sales in June and December.

Highest profit was made in October.

Made its major loss in month February.

![Screenshot 2024-06-08 175142](https://github.com/Vickeejai/Sales-Report/assets/133552578/daeeb338-7e27-4cff-a7cc-6702e1668643) 

**BIRO:**
A growth for the last quarter of the year for all parameters.

A B C Stationery experienced their highest Sales Proportion and highest Number of Sales in June and December.

Highest profit was made in December.

Made its major loss in moth August

![Screenshot 2024-06-08 175254](https://github.com/Vickeejai/Sales-Report/assets/133552578/436bcd1b-6a52-4a5e-ac07-53c5637bfc69)

**MARKERS:**
There was a major decline for all parameters for markers in the year 2014.

A B C Stationery invested so much in this product but got no returns.

They got profit for both July and October, but made their highest in July.

Mostly losses made.

![Screenshot 2024-06-08 175358](https://github.com/Vickeejai/Sales-Report/assets/133552578/77ea2d3f-af68-4194-ba4d-bcbb365e16cb)

**NOTEPADS:**
There was a major decline for all parameters for Notepads in the year 2014.

A B C Stationery invested so much in this product but got no returns.

They made profit in August

Mostly losses made.

![Screenshot 2024-06-08 175557](https://github.com/Vickeejai/Sales-Report/assets/133552578/28666894-cd89-4028-8167-7d8ce5d48ef8)

**PENCILS:**
A growth for the first quarter of the year for all parameters.

A B C Stationery experienced their highest Sales Proportion and highest Number of Sales in June and December.

Highest profit was made in April.

Made its lowest profit in February.

![Screenshot 2024-06-08 175641](https://github.com/Vickeejai/Sales-Report/assets/133552578/dfb14359-2bd3-4126-99aa-f68662edf86d)

**STAPLERS:**
There was a major decline for all parameters for Stapler in the year 2014.

A B C Stationery invested so much in this product but got no returns.

They made profit in September

Mostly losses made.

![Screenshot 2024-06-08 175809](https://github.com/Vickeejai/Sales-Report/assets/133552578/bb4654e8-91d8-4edc-80d3-012d95229e9d)

4. Based on product category, the highlights for year on year results at Quarter 4 is described below:
Biro, A4 Paper and Pencils produced significant revenue and profits with low and reasonable manufacturing cost in progression from 2013 to 2014, Staplers and Notepads showed huge lossses from the analysis with time even with the high amount of manufacturing cost, and Markers produced profit in 2013 but losses in 2014.

![Screenshot 2024-06-10 111500](https://github.com/Vickeejai/Sales-Report/assets/133552578/d01740b3-e8c7-4d95-ab3b-178be97f348c)

The analysis shown for state comparing 2013 and 2014, Osun, Ogun and Oyo state are generating more profit in most product lines compared to Lagos and Ondo state.

![Screenshot 2024-06-10 114231](https://github.com/Vickeejai/Sales-Report/assets/133552578/61004008-488a-492a-917a-9ddfa4804675)

5. The key drivers of performance are Biro, A4 Paper, Pencil

6. The products to be discontinued due to poor outcomes are Staplers, Notepads, and Markers.

7. The products in which the highest tax is been paid for each state, each segment and overall is BIRO

![Screenshot 2024-06-08 200930](https://github.com/Vickeejai/Sales-Report/assets/133552578/56f36b07-330b-4442-a4bd-ec2b41cf0960)

### **Prescriptive Analytics**

 - Based on our Descriptive and Diagnostic Analysis of this business, we recommend that A B C Stationary company should continue in the production of Biro, A4 Paper and Pencil because it will make and not mar the company by maximizing profit.
  - An Audit on all their financial records with regards to the products and segments in view should take place due to the fact that there is a rampant occurrence of the manufacturing cost either higher or the same with the revenue gotten.
 - We also recommend that there should be a slight increase in the selling price of products because it looks like the economy is affecting their output negatively.
 - An audit on all sections in the company for the inspection of any fraudulent activity should be carried out in the respective departments.
 - A market research or survey should be conducted by A B C Stationary to get feedback from their end users on how to improve their products.
 - The production of Staplers, Markers and Notepads should be suspended indefinitely because it is producing no significant revenue even with high manufacturing cost.

   By following these steps, A B C Stationary will be able to have reasonable profits in years to come.



























