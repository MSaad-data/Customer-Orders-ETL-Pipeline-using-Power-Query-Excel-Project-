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
