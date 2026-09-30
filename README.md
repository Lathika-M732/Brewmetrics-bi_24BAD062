# BrewMetrics BI

A version-controlled Business Intelligence solution for BrewMetrics Coffee Co. using Power BI, GitHub, and GitHub Copilot.

## Project Overview

BrewMetrics Coffee Co. operates Flagship stores, Kiosks, and Drive-Thrus across four cities. This project analyzes sales data from April to June to identify sales trends, seasonal patterns, product performance, and differences in city-level performance.

The project is developed using a version-controlled workflow so that changes to the data model, DAX measures, dashboard, and documentation can be tracked through Git commits.

## Tools Used

- Power BI Desktop
- Power BI Project (.pbip)
- GitHub
- GitHub Desktop / Git
- Visual Studio Code
- GitHub Copilot
- Power Query
- DAX

## Dataset

The project uses the `brewmetrics_sales.csv` dataset.

The dataset contains transaction-level sales information including:

- Date
- City
- Store Format
- Category
- Item
- Quantity
- Unit Price
- Sales Amount

The data contains approximately 15,500 transactions covering April to June.

## Data Model

The flat sales data is transformed into a Star Schema.

### Fact Table

**Fact_Sales**

Contains transaction-level sales information such as:

- Date
- City
- Store Format
- Item
- Quantity
- Unit Price
- Sales Amount

### Dimension Tables

**Dim_Date**

Contains date-related information such as:

- Date
- Year
- Month
- Month Number
- Day

**Dim_City**

Contains city information used for city-level analysis.

**Dim_Product**

Contains product and category information used for product-level analysis.

### Star Schema

```text
                 Dim_Date
                    |
                    |
Dim_City ---- Fact_Sales ---- Dim_Product
                    |
                    |
              Store Format
