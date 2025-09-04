
This project analyzes the operations of **Behind the Scenes Clothing Retail (BTSCR)**. The goal was to help senior management understand the key drivers of the business by analyzing Stores, Products, and Orders, and visualizing insights for better decision-making.

---

## Project Overview
As a Data Analyst, I worked on:

- Importing and exploring CSV data extracts for Stores, Products, Transactions, and Shipping.
- Cleaning and transforming data to prepare it for analysis.
- Calculating key business metrics for Stores, Products, and Orders.
- Visualizing insights to identify trends, outliers, and key performance drivers.

---

## Features

### Data Loading & Exploration
- Import four CSV files into Pandas DataFrames.
- Identify and handle missing values efficiently.
- Fill missing unique identifiers sequentially and assign default values to missing Shipping information (`Expedited`).

### Data Cleaning
- Added new stores to create a complete `stores_df`.
- Combined store DataFrames.
- Dropped duplicate rows from `transactions_df`.
- Converted `OrderID` to integer and `Year`, `Month`, `Day` to string.
- Split `Name` column in `products_df` into `Type` and `Colour`.
- Standardized colour values (`Gray` → `Grey`).

### Data Transformation
- Created `orders_df` by merging transactions, products, shipping, and store data.
- Added new columns:
  - `Date` (from Year, Month, Day)
  - `Discount Pct` (30% for green or grey socks)
  - Metrics: `Sale Price`, `Net Profit`, `Total Revenue`, `Total Cost`, `Total Net Profit`

### Data Analysis
- **Store Metrics:** Total Revenue, Total Cost, Net Profit, order counts by Store and City.
- **Product Metrics:** Top-selling products, products with highest Revenue-to-Cost ratio, Total Revenue and Total Net Profit.
- **Order Metrics:** Analysis of first 200 transactions, multiple product orders, and mean Quantity by Colour and City.

### Data Visualization
- **Bar Plots:** Quantity sold by ProductID, average Discount Pct by City.
- **Scatter Plots:** Total Revenue vs Total Cost with Net Profit hue.
- **Line Plots:** Total Net Profit over time.
- **Box Plots:** Total Revenue by product Type to identify outliers.
- **Correlation Matrix & Heatmap:** Analyze relationships between metrics.
- **Outlier Detection:** Identified outliers using the IQR rule for further investigation.

---

## Data
The analysis uses four CSV files:

- `stores.csv`
- `products.csv`
- `transactions.csv`
- `shipping.csv`

---

## Notebook Preview
You can view the Jupyter Notebook directly on GitHub without downloading:  
[view Notebook](https://github.com/JaviGARES/Python--Behind-the-Scenes-Clothing-Retail--Case-Study.ipynb)


---


## Key Skills
- Data Cleaning & Transformation
- Merging and Joining DataFrames
- Calculating business metrics
- Visualizing data using bar plots, scatter plots, line charts, box plots, and heatmaps
- Outlier detection and analysis


