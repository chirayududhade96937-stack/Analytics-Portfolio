# Fuelling the Future: Strategic Insights and Forecasts for Australia's Petroleum Export Landscape

**Author:** Chirayu Dudhade 
**Course:** 32146 - Data Visualisation and Visual Analytics  
**Project Type:** Visual Analytics & Forecasting  
**Date:** June 2025

---

## Project Overview

This project provides a comprehensive visual analytics study of **Australia's international trade** from 1988 to 2024, with a focus on **Mineral Fuels (Category 3)**, particularly **Petroleum (Subcategory 33)**. The goal is to deliver actionable insights and strategic forecasts for policymakers and industry stakeholders, combining **data-driven analysis** with **interactive visualizations**.

---

## Key Objectives

- Analyse Australia’s historical import and export trends in petroleum and energy commodities.
- Identify critical fluctuations, structural shifts, and patterns within the energy sector.
- Forecast petroleum exports from 2025–2029 under different geopolitical and global demand scenarios.
- Provide actionable recommendations for infrastructure investment, financial resilience, energy diversification, and policy adaptability.
- Leverage **dashboards** and **storyboards** to communicate complex insights effectively.

---

## Dataset

- **Source:** Australian Bureau of Statistics (ABS)  
- **Years:** 1988–2024  
- **Scope:** 10 major trade categories, 67 subcategories, import and export values (A$ million)  
- **Focus Category:** Mineral Fuels, Lubricants & Related Materials (Category 3)  
- **Focus Subcategory:** Petroleum Products (Subcategory 33)

---

## Methodology

### 1. Data Preparation & Transformation

- Merged import and export datasets into a unified structure.
- Created separate sheets for:
  - **Raw dollar values**
  - **Analytical trends (YoY change)**
  - **Statistical proportions**
- Ensured data integrity: no missing values, duplicates, or outliers.

### 2. Analytical Techniques

- Year-over-Year Change Analysis:  
  `Annual Change = ((Current Year - Previous Year) / Previous Year) * 100`
- Proportional ratios for subcategories and categories relative to total trade.
- Indexed trade value trends to uncover long-term growth and volatility patterns.

### 3. Visualization & Storytelling

- **Dashboards:** Interactive tools for granular exploration of trade data, trends, and outliers.  
<img width="995" height="792" alt="image" src="https://github.com/user-attachments/assets/dd9b913c-bae8-44ad-ab3b-620716e18993" />

- **Storyboards:** Narrative-driven visualizations highlighting historical transformations, turbulent events, and future projections.  
<img width="1652" height="831" alt="image" src="https://github.com/user-attachments/assets/748c3442-47ba-45ef-821d-dace87e52c37" />


### 4. Forecasting & Strategic Scenarios

- Trend projections for petroleum exports (2025–2029).
- Scenario matrix evaluating four potential futures:
  - **Boom Rebound** – High demand, high stability
  - **Volatile Riches** – High demand, low stability
  - **Green Phaseout** – Low demand, high stability
  - **Global Breakdown** – Low demand, low stability

---

## Key Insights

### Historical Trends (1988–2014)

- Petroleum imports rose 23×, highlighting dependence on imported fuels.
- Natural gas exports surged 90×, emerging as a key global player in LNG markets.
- Coal exports plateaued while petroleum exports fluctuated with global oil prices.
<img width="652" height="334" alt="image" src="https://github.com/user-attachments/assets/fc683ece-37f3-4b77-81ca-256d35e38a64" />

### Recent Dynamics (2015–2024)

- Petroleum exports showed extreme volatility due to global shocks: 2016 oil crash, 2020 COVID-19 pandemic, 2022 Ukraine conflict.
- LNG exports consistently increased, surpassing petroleum as Australia’s most valuable energy export.
<img width="650" height="402" alt="image" src="https://github.com/user-attachments/assets/76f90dc7-f282-4068-9ee3-5a302dc15faa" />


### Forecast (2025–2029)

- Petroleum exports projected to grow steadily from $16.7B (2025) to $20.1B (2029).
- Strategic planning crucial under varying global demand and geopolitical conditions.
<img width="593" height="362" alt="image" src="https://github.com/user-attachments/assets/63e6622b-53ff-4ef4-a706-64740e8fdf26" />


---

## Recommendations

1. **Invest in Export Infrastructure** – Expand capacity and trade logistics to capitalize on high-growth scenarios.
2. **Build Financial Resilience** – Implement price-hedging strategies and maintain financial buffers.
3. **Diversify Energy Portfolio** – Invest in renewable and alternative fuels in anticipation of the Green Phaseout scenario.
4. **Enhance Policy & Trade Flexibility** – Develop agile policies to navigate geopolitical and demand-based shocks.

---

## Visualizations

- **Stacked Area Charts:** Evolution of coal, petroleum, and gas exports.  
<img width="569" height="357" alt="image" src="https://github.com/user-attachments/assets/aaaa058a-9e79-4982-8a48-543ef601db57" />

- **Dual-Line Charts:** Comparison of petroleum vs LNG exports and trends.
<img width="615" height="346" alt="image" src="https://github.com/user-attachments/assets/dbb07aa3-0ed2-4fc5-b3a8-239f9c6fe19b" />

- **Box Plots:** Export volatility analysis.
<img width="628" height="382" alt="image" src="https://github.com/user-attachments/assets/4f3b72d1-3c5d-467a-ab21-075856fe45b8" />

- **Waterfall Chart:** Cumulative gains/losses over key years.
<img width="584" height="360" alt="image" src="https://github.com/user-attachments/assets/cb41feda-cd60-49b4-83eb-4b6393145301" />

- **Scenario Matrix:** Strategic outlook based on global demand and geopolitical stability.
<img width="621" height="383" alt="image" src="https://github.com/user-attachments/assets/58d72d40-4b0d-4555-a331-12c8cf9fae57" />


_Interactive dashboards were developed using Tableau to complement narrative storyboards._

---

## Tools & Technologies

- **Data Processing:** Microsoft Excel (data cleaning, transformation, YoY calculations)  
- **Visualization & Dashboards:** Tableau (interactive dashboards and storyboards)  
- **Statistical Analysis:** Descriptive statistics, index calculations, proportional ratios

---

## Conclusion

This project integrates historical analysis, volatility assessment, forecasting, and scenario planning to provide strategic insights into Australia’s petroleum export sector. By combining dashboards and storyboards, it offers both interactive exploration and narrative clarity, empowering policymakers and industry stakeholders to make informed, resilient decisions in a dynamic global energy landscape.

---

## Project Structure

```text
├── .gitignore
├── README.md
|
├── data/
│   ├── raw/
│   │   ├── australia_trade_raw.xlsx
│   │   └── petroleum_exports.csv
│   └── processed/
│       └── processed_data.xlsx
|
├── scripts/
│   ├── data_cleaning.py
│   └── sql_transformation_queries.sql
|
├── models/
│   └── petroleum_analytics.pbix
|
├── dashboards/
│   ├── petroleum_vs_LNG.twb
│   └── energy_export_dashboard.twb
|
├── reports/
│   └── assessment3_report.pdf
|
└── visuals/
    ├── chapter1/
    ├── chapter2/
    └── chapter3/
