# Walmart Sales Dashboard (Power BI)

## Description  
This repository contains a Power BI dashboard developed to analyze Walmart sales data across multiple stores, time periods, and economic factors. The project focuses on transforming raw retail data into interactive visual insights for performance evaluation and decision-making.

---

## Dataset  
- Source: Kaggle Walmart Sales Dataset  
- Time Period: 2010–2012  
- Stores: 45  
- Records: ~1,000  

---

## Features  
- KPI metrics including Total Sales, Average Weekly Sales, and Holiday Sales  
- Monthly sales trend analysis  
- Store-wise performance comparison  
- Holiday vs non-holiday sales distribution  
- Fuel price vs sales correlation analysis  
- Temperature variation across stores  
- Interactive filters for year and store selection  

---

## Dashboard Preview  
![Dashboard Screenshot](./assets/dashboard.png)

---

## Data Processing  
- Date format correction using locale settings  
- Data type standardization for numerical and categorical fields  
- Creation of Month Name and Month Number columns  
- Holiday classification using DAX  
- Proper sorting of time-based data  

---

## DAX Measures  
```DAX
Total Sales = SUM('Walmart'[Weekly_Sales])

Avg Weekly Sales = AVERAGE('Walmart'[Weekly_Sales])

Total Stores = DISTINCTCOUNT('Walmart'[Store])

Holiday Sales =
CALCULATE(
    SUM('Walmart'[Weekly_Sales]),
    'Walmart'[Holiday_Flag] = 1
)

Non Holiday Sales =
CALCULATE(
    SUM('Walmart'[Weekly_Sales]),
    'Walmart'[Holiday_Flag] = 0
)
```

---

## Tech Stack  
- Power BI Desktop  
- Power Query  
- DAX (Data Analysis Expressions)  
- Microsoft Excel  

---

## Key Insights  
- Sales peak mid-year and decline towards year-end  
- Majority of sales occur during non-holiday periods  
- Significant variation exists in store performance  
- Fuel price shows a weak negative correlation with sales  
- Temperature varies across store locations  

---

## Future Improvements  
- Integration of the complete dataset  
- Geographic visualization of store performance  
- Inclusion of additional economic indicators  
- Forecasting and drill-through analysis  
- Mobile layout optimization  

---

## Repository Structure  
```
├── data/               # Dataset files
├── assets/             # Dashboard screenshots
├── Walmart.pbix        # Power BI file
└── README.md
```

---

## Author  
Sounak Bhattacharyya  
B.Tech Computer Science and Engineering  
