# Customer-Orders-ETL-Pipeline-using-Power-Query-Excel-Project-
This project focuses on building an end-to-end ETL pipeline using Excel Power Query Editor. The dataset contains customer order transactions including products, pricing, shipping, regions, and dates. The goal is to extract raw data, apply structured transformations, and load clean, analysis-ready data.


## **Data Extraction**

Downloaded the raw customer orders dataset from Kaggle

Imported the dataset into Excel using Get Data (Power Query)

Loaded the data into Power Query Editor instead of directly into a worksheet

Used the imported file as the single source of truth for all transformations


## **Data Transformation** (Power Query Editor)

Extracted the raw customer orders dataset into Excel Power Query Editor

Verified and fixed data types across all columns to ensure transformation accuracy

Identified missing values (nulls) in Age and Region and handled them without distorting the source data

Created a Calculated Total Price column using Unit Price × Quantity to validate data integrity

Compared the original Total Price with the calculated values and identified inconsistencies

Added a Price Validation column to flag mismatched records instead of deleting them

Derived Order Year and Order Month from Order Date for time-based analysis

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/a9389af9-1055-4652-be97-d3b588e1ce71" />


Created a reference query to preserve raw transformed data and applied Group By to aggregate total revenue by Region using calculated values. Handled missing dimension values by standardizing null Regions as Not Specified to preserve revenue integrity during aggregation. 

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/2bfdad2e-232a-40a6-beb9-daac565f39b2" />


Aggregated total revenue, total quantity, and average unit price by Product Category for business-ready summaries

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/a44b9d40-1b10-489c-a386-477c8f125fbf" />


Aggregated total revenue and number of orders per customer to analyze customer-level performance












