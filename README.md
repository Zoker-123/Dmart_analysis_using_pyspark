# DMart Sales Data Analysis Using PySpark

## Overview
This project implements a PySpark pipeline to analyze DMart sales data from three CSV files: `Products.csv`, `Sales.csv`, and `Customers.csv`. It processes, cleans, and joins the data to answer 10 analytical business questions, delivering results in a tabular format. The pipeline is structured into five tasks, with modular query definitions and execution, ensuring scalability and clarity.

## Problem Statement
- **Objective**: Develop a robust pipeline to load, transform, and analyze sales data for actionable insights.
- **Tasks**:
  - **Task 1**: Initialize a PySpark session.
  - **Task 2**: Load CSV files into DataFrames.
  - **Task 3**: Clean, transform, and join DataFrames into an integrated dataset.
  - **Task 4**: Formulate 10 analytical questions as query functions.
  - **Task 5**: Execute queries and display results in tables.

## Technologies Used
- **PySpark**: For distributed data processing and Spark SQL queries.
- **Python**: Core scripting language.
- **Jupyter Notebook**: Optional for interactive execution and PDF export.
- **CSV Files**: Input datasets.

## Dataset
The project uses three CSV files located in `C:\Guvi\Project_5`:
- **Products.csv** (1862 rows):
  - Columns: `Product ID`, `Category`, `Sub-Category`, `Product Name`
- **Sales.csv** (9994 rows):
  - Columns: `Order Line`, `Order ID`, `Order Date`, `Ship Date`, `Ship Mode`, `Customer ID`, `Product ID`, `Sales`, `Quantity`, `Discount`, `Profit`
- **Customers.csv** (793 rows):
  - Columns: `Customer ID`, `Customer Name`, `Segment`, `Age`, `Country`, `City`, `State`, `Postal Code`, `Region`

## Project Structure
- `dmart_sales_analysis.py`: Main script containing the full pipeline and analysis.
- `dmart_analysis.ipynb`: Optional Jupyter Notebook for interactive execution and PDF export.
- `README.md`: Project documentation (this file).
- `.gitignore`: Excludes CSV files, notebook checkpoints, and temporary files (e.g., `__pycache__`, `*.csv`, `.ipynb_checkpoints/`).

## Analytical Questions
The pipeline answers the following questions, with results displayed in tabular format:

- Total sales for each product category.
- Customer with the highest number of purchases.
- Average discount given across all sales.
- Unique products sold in each region.
- Total profit generated in each state.
- Product sub-category with the highest sales.
- Average age of customers in each segment.
- Orders shipped in each shipping mode.
- Total quantity of products sold in each city.
- Customer segment with the highest profit margin.

## Insights
- **Revenue Drivers**: High-sales categories indicate key product lines to prioritize.
- **Customer Behavior**: Top purchasers suggest opportunities for loyalty programs.
- **Profitability**: Regional and state-level profit data highlight strong markets.
- **Operational Efficiency**: Shipping mode distribution informs logistics optimization.
