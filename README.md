# Zepto SQL Data Analysis 🛒

## Project Overview

This project explores Zepto product inventory data using **SQL, Python, and SQLite** to uncover useful business insights related to product pricing, discounts, stock availability, and inventory management.

The project involves data exploration, data cleaning, and business-oriented SQL queries to understand product-level and category-level performance.

## Objectives

- Explore and understand the product inventory dataset.
- Identify distinct product categories and stock availability.
- Detect duplicate product names and inspect missing values.
- Clean and standardize product pricing data.
- Identify products offering the highest discounts.
- Estimate revenue across product categories.
- Analyze product value using price-per-gram calculations.
- Categorize products by weight and calculate inventory weight by category.

## Technologies Used

- **SQL** — Data querying, filtering, aggregation, and business analysis
- **Python** — Data handling and database integration
- **Pandas** — Data loading and DataFrame operations
- **SQLite** — Storing and querying product inventory data
- **Jupyter Notebook / Google Colab** — Development environment

## Project Workflow

### 1. Data Loading
Loaded the Zepto dataset from a CSV file using Pandas and prepared it for analysis.

### 2. Database Setup
Created an SQLite database and stored the dataset in a table named `zepto`. Used a Python helper function to execute SQL queries and display their results.

### 3. Data Exploration
- Counted the records in the dataset.
- Inspected sample records and missing values.
- Identified distinct product categories.
- Examined in-stock and out-of-stock products.
- Identified product names appearing multiple times.

### 4. Data Cleaning
Converted MRP and discounted selling prices from their original stored units into rupees by dividing the values by 100.

### 5. Business Analysis
Wrote SQL queries to answer eight business questions related to discounts, inventory, pricing, revenue, and product categories.

## Business Questions Solved

| No. | Business Question | SQL Concepts |
|---|---|---|
| 1 | What are the top 10 products by discount percentage? | `ORDER BY`, `LIMIT` |
| 2 | Which out-of-stock products have the highest MRP? | `WHERE`, `ORDER BY` |
| 3 | What is the estimated revenue for each category? | `SUM()`, `GROUP BY` |
| 4 | Which products have an MRP above ₹500 and a discount below 10%? | `WHERE`, comparison operators |
| 5 | Which five categories have the highest average discount? | `AVG()`, `GROUP BY`, `LIMIT` |
| 6 | Which products above 100 grams offer the lowest price per gram? | Calculated columns, filtering, sorting |
| 7 | How can products be grouped into low, medium, and bulk weight categories? | `CASE WHEN` |
| 8 | What is the total inventory weight for each category? | `SUM()`, `GROUP BY` |

## Key Analysis Areas

- **Discount Analysis:** Compare product discount percentages and identify highly discounted products.
- **Inventory Analysis:** Examine stock availability and identify expensive products that are out of stock.
- **Revenue Analysis:** Estimate category-level revenue using discounted selling price multiplied by quantity.
- **Price and Value Analysis:** Calculate price per gram to compare products by value.
- **Category Analysis:** Compare average discounts and total inventory weight across categories.
- **Data Quality:** Inspect missing values and repeated product names.

## SQL Skills Demonstrated

`SELECT` · `WHERE` · `ORDER BY` · `LIMIT` · `GROUP BY` · `SUM()` · `AVG()` · `COUNT()` · `DISTINCT` · `CASE WHEN` · Aggregate Functions · Data Cleaning · Business Analysis

## Repository Structure

```text
zepto-sql-data-analysis/
│
├── sql_project.ipynb
├── zepto_v2.csv          # Input dataset, if permitted to share
└── README.md
```

The CSV file should be included only if you have permission to redistribute the dataset.

## How to Run the Project

1. Clone or download this repository.
2. Open `sql_project.ipynb` in Jupyter Notebook or Google Colab.
3. Install the required Python libraries:

   ```bash
   pip install pandas
   ```

4. Make sure the `zepto_v2.csv` dataset is available in the working directory, or upload it when prompted in Google Colab.
5. Run the notebook cells sequentially to create the SQLite database and execute the SQL queries.

**Note:** The notebook uses Python's built-in `sqlite3` module, so a separate SQLite installation is generally not required.

## Conclusion

This project demonstrates how SQL can be used to explore retail inventory data and answer practical business questions. By combining SQL queries with Python and SQLite, the analysis covers pricing, discounts, estimated revenue, product value, and inventory management.

It showcases practical skills in data exploration, data cleaning, SQL aggregation, conditional logic, and business-oriented data analysis.

## Author

Created as a hands-on SQL and data analysis project to practice querying structured data and deriving business insights.
