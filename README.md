Walmart Sales Dashboard (Power BI)
Overview

This project presents a Power BI dashboard developed to analyze Walmart sales data across multiple stores, time periods, and economic factors. The objective is to transform raw transactional data into meaningful insights for business decision-making.

Problem Statement

Retail datasets often contain complex patterns influenced by time, holidays, and external economic variables. This project addresses key questions related to sales trends, store performance, and the impact of factors such as fuel price and temperature.

Dataset
Source: Kaggle Walmart Sales Dataset
Time Period: 2010–2012
Stores: 45
Records: ~1,000
Features include Weekly Sales, Temperature, Fuel Price, CPI, and Unemployment
Key Features
Total Sales: 6.74 Billion
Average Weekly Sales: 1.05 Million
Holiday Sales: 505.30 Million
Store-level performance comparison
Monthly sales trend analysis
Holiday vs non-holiday sales distribution
Fuel price vs sales correlation analysis
Temperature variation across stores
Interactive filtering by year and store
Data Processing
Corrected date format using locale settings
Converted columns to appropriate data types
Created Month Name and Month Number columns
Generated Holiday Type using DAX
Ensured proper sorting of time-based data
DAX Measures
Tools and Technologies
Power BI Desktop
Power Query
DAX
Microsoft Excel
Kaggle Dataset
Insights
Sales are highest during mid-year and lowest towards year-end
A majority of sales occur during non-holiday periods
Certain stores significantly outperform others
Fuel price shows a weak negative correlation with sales
Temperature varies notably across store locations
Future Improvements
Integration of full dataset
Geographic visualization of stores
Additional economic indicators (CPI, unemployment)
Forecasting and drill-through analysis
Mobile layout optimization
