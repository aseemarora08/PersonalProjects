# PersonalProjects

# Sales Analysis Overview

## About the Dataset: Sales Data

Source:https://www.kaggle.com/datasets/beekiran/sales-data-analysis
The dataset used in this analysis comprises 11 columns, each representing a distinct attribute related to product purchases. Below is an overview of these columns:

1. **Order ID:** A unique identifier assigned to each order placed for a product.
2. **Product:** The item that has been purchased.
3. **Quantity Ordered:** Indicates the quantity of the product ordered in each transaction.
4. **Price Each:** Represents the unit price of the product.
5. **Order Date:** The date when the purchase order was placed.
6. **Purchase Address:** The shipping address where the order is to be delivered.
7. **Month:** Derived attribute indicating the month of the purchase.
8. **Sales:** Derived attribute representing the total sales amount for each transaction.
9. **City:** Derived attribute specifying the city associated with the purchase.
10. **Hour:** Derived attribute indicating the hour of the day when the purchase order was placed.

## About the Dataset: Income
Source: https://www.kaggle.com/datasets/goldenoakresearch/us-household-income-stats-geo-locations

The database contains 32,000 records on US Household Income Statistics & Geo Locations. The field description of the database is documented in the attached pdf file. To access, all 348,893 records on a scale roughly equivalent to a neighborhood (census tract) see link below and make sure to up vote. Up vote right now, please.

## Analysis Phases

### Phase 1: Reading and Cleaning the Data

This phase involves reading the sales data from a CSV file, inspecting data types, converting 'Order Date' to datetime format, and extracting components like 'Order Time' and 'Order Date' for further analysis.

### Phase 2: Wrangling

#### Computing Products and their Sales

In this section, total sales for each product are calculated, and a new column 'Total Sales' is added. Duplicate rows based on the 'Product' column are removed, and the resulting data is sorted by 'Total Sales' in descending order. An Altair bar chart is then plotted to visualize the total sales for each product.

#### Studying MacBook Purchasing Patterns and Trends

This section focuses on analyzing purchasing patterns for MacBook Pro Laptops. Regional sales are calculated, and the geographical distribution of sales is visualized on a world map using GeoPandas. Additionally, the relationship between the month, total sales, and hourly sales is explored through Altair scatter plots.

#### Drawing Relation between Incomes and Average Spendings

Income data is incorporated into the analysis, and the relationship between average income and total sales for different cities is visualized using an Altair scatter plot.

## Code and README File

The corresponding code file (Python script) provides a step-by-step implementation of the above phases, using libraries such as Pandas, Altair, GeoPandas, and more. For more detailed explanations and visualizations, refer to the comments within the code file. The README file associated with this analysis provides additional context, instructions on data sources, and guidance on running the code on different environments. Ensure to check the README for a comprehensive understanding of the analysis.
