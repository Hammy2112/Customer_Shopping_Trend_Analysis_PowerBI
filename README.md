# Power BI Dashboard: Customer Shopping Trends Analysis

## 📌 Project Overview

As a Data Analyst for a retail chain, this project focuses on transforming raw customer shopping data into an interactive Power BI dashboard. The objective is to uncover actionable insights regarding purchase patterns, customer segmentation, and geographic performance to drive targeted marketing strategies for the upcoming retail season.

## 🗄️ Data Engineering & ETL (Power Query)

The raw dataset was extracted directly from a web source into Power BI Desktop. To ensure data quality and optimize the model for visualization, several transformation steps were executed in Power Query:

* **Column Normalization:** Renamed tables and standardizing column headers for clarity.
* **Data Cleansing:** Removed redundant and irrelevant columns to reduce model size.
* **Feature Engineering:** Split combined strings (e.g., separating `Color-Size` into distinct `Color` and `Size` attributes).
* **Data Type Formatting:** Corrected structural issues, specifically parsing text-based review ratings and converting them into calculable decimal values.

## 🧮 Data Modeling & DAX

To facilitate deeper demographic analysis, custom DAX (Data Analysis Expressions) was utilized to create calculated columns, notably grouping raw customer ages into distinct **Age Categories** for cohort analysis.

## 📊 Dashboard Modules & Visualizations

The interactive dashboard is divided into three core analytical focus areas:

### 1. Customer Demographics Analysis

* **Age Distribution:** Visualizing the spread of the customer base across the newly created DAX age categories.
* **Loyalty Profiling:** Identifying which specific age groups exhibit the highest brand loyalty based on historical purchase frequency.
* **High-Value Segments:** Highlighting the specific demographic cohorts responsible for the highest-value individual transactions.
* **Gender Dynamics:** Analyzing how purchase frequency and behavior vary between male and female shoppers.

### 2. Product & Seasonal Trends

* **Revenue Drivers:** Isolating and highlighting the top 2 product categories generating the highest overall sales volume.
* **Seasonality:** Tracking spending trends across different seasons to identify peak revenue periods.

### 3. Geographical & Shipping Analysis

* **Location Mapping:** A custom gradient map visualizing customer distribution and comparing total purchase amounts by region.
* **Logistics Preferences:** Assessing the popularity of different shipping methods across the top five highest-revenue countries.

## 🎛️ Interactive Features

The dashboard is designed for management to explore the data dynamically:

* **KPI Cards:** Tracking top-line metrics at a glance, including **Total Sales**, **Average Purchase Amount**, and **Average Rating**.
* **Dynamic Slicers:** Allowing users to filter the entire report canvas by `Category`, `Location`, `Age Segment`, and `Gender`.
