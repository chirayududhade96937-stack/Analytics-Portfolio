# Strategic Retail Growth & Revenue Diagnostics Using Power BI

![Project](https://img.shields.io/badge/Project-Visual_Analytics-blue)
![Power BI](https://img.shields.io/badge/Tool-Power_BI-yellow?logo=power-bi&logoColor=black)
![DAX](https://img.shields.io/badge/Focus-DAX_&_Data_Modeling-blueviolet)
![Forecasting](https://img.shields.io/badge/Analysis-Time_Series_Forecasting-red)

**Author:** Chirayu Dudhade  
**Project Type:** Business Intelligence & Strategic Analysis  
**Dataset:** UCI Online Retail (UK-based gift retailer)  
**Period Covered:** Dec 2010 – Dec 2011  

---

## 📌 Project Overview

This project analyzes transactional data from a UK-based online gift retailer to answer a single strategic question:

**“Where should the business focus to grow revenue sustainably while reducing operational leakage?”**

Using over **540,000 real-world transactions**, the analysis goes beyond descriptive reporting. The project builds a structured semantic layer, identifies high-efficiency customers and markets, diagnoses operational friction, and converts historical performance into forward-looking growth decisions.

The result is a **four-page executive Power BI dashboard** designed to mirror how leadership teams actually consume analytics:  
from *understanding performance* → *identifying value* → *fixing inefficiencies* → *planning growth*.

---

## 🧠 Analytical Story Arc (4-Page Dashboard)

### Page 1 – Business Performance Pulse  
**Purpose:** Establish trust in the numbers and set a clear baseline.

This page answers the foundational question:  
**“What is happening in the business?”**

**Key insights:**
- Revenue, order volume, and cancellations establish overall scale and volatility
- Time-series trends reveal clear seasonality
- Category contribution highlights concentration risk

**Key finding:**  
While the business achieves strong overall revenue, it is **heavily dependent on the Home Decor category**, contributing over **35% of total revenue**. Additionally, a **sharp spike in cancellations during April** signals a potential operational or supply chain issue rather than random noise.

**Narrative takeaway:**  
Before discussing growth, leadership must understand where revenue truly comes from and where it is leaking.

<img width="947" height="737" alt="image" src="https://github.com/user-attachments/assets/1478a425-5e2c-4638-bedd-b6524e42bdd0" />

---

### Page 2 – Customer Insights & VIP Analysis  
**Purpose:** Identify who drives profitability and where retention matters most.

Once the performance baseline is established, the analysis shifts from *what* is happening to *who* is driving it.

**Approach:**
- RFM-style segmentation isolates high-value (VIP) customers
- Repeat purchase behavior is analyzed across countries
- Average Order Value (AOV) is used to assess efficiency, not just scale

**Key finding:**  
The **Netherlands** emerges as a standout high-efficiency market. Despite lower absolute volume than the UK, Netherlands-based VIP customers demonstrate a **repeat purchase rate exceeding 70%**, significantly outperforming the domestic average.

**Narrative takeaway:**  
Retention in the right markets is a lower-risk growth lever than broad acquisition. Not all revenue is equally valuable.

<img width="945" height="738" alt="image" src="https://github.com/user-attachments/assets/28edfa05-fbbf-4c7f-a055-938638d0d928" />

---

### Page 3 – Operational Efficiency & Diagnostics  
**Purpose:** Identify where revenue is lost through inefficiency or dead stock.

This page functions as a diagnostic health check.

**Key visuals and logic:**
- A **Sales Quantity vs Unit Price scatter plot** classifies products into:
  - High-volume “Stars”
  - Low-volume, low-impact laggards
- A **Decomposition Tree** breaks down cancellation-driven revenue leakage

**Key finding:**  
Approximately **$0.7M in revenue leakage** can be traced to a small number of categories and countries. The issue is concentrated, not systemic — which makes it actionable.

**Narrative takeaway:**  
Growth does not require adding complexity. It requires removing friction and reallocating attention away from underperforming SKUs.

<img width="947" height="732" alt="image" src="https://github.com/user-attachments/assets/bebacfe7-5719-4c71-835c-0f0ee6224660" />

---

### Page 4 – Strategic Growth & Forecasting  
**Purpose:** Convert historical insight into forward-looking decisions.

The final page moves from diagnosis to strategy.

**Key components:**
- **Time-series revenue forecasting** using exponential smoothing with confidence intervals
- Category-level Month-over-Month (MoM) growth comparison
- International market efficiency analysis combining:
  - Revenue
  - AOV
  - Customer retention

**Key finding:**  
Based on recent trends, **Home Decor shows strong positive MoM momentum**, while international efficiency metrics reinforce **Netherlands and EIRE** as the most defensible expansion corridors.

**Narrative takeaway:**  
Growth is only real if it is repeatable, efficient, and retention-driven.

<img width="947" height="737" alt="image" src="https://github.com/user-attachments/assets/1a92c847-6d76-4862-a471-ff6f90ee5ae5" />

---

## 🛠️ Technical Implementation

### 1. Semantic Data Engineering
The raw dataset contains unstructured product descriptions with no usable categories.  
To solve this, I engineered a **keyword-to-category mapping table with priority logic**, allowing product descriptions to be consistently translated into business-ready entities.

**Why this matters:**
- Separates business logic from calculations
- Improves transparency and auditability
- Allows category definitions to scale without rewriting DAX

Over **90% of revenue** was cleanly classified, keeping the “Other” category statistically insignificant.

---

### 2. Core Metrics & DAX Logic
Key measures were designed to remain accurate under heavy cross-filtering:

- **Net Revenue:** Accounts for cancellations and unit price variation
- **Rolling Retention:** Evaluates customer loyalty within a 90-day window
- **MoM Growth Index:** Normalizes growth comparisons across categories and markets

All calculations were built with defensive logic to ensure consistency across pages.

---

## 📈 Business Impact & Recommendations

This project demonstrates the shift from **data reporting to decision support**.

**Key recommendations:**
1. **Address April operational friction** to reduce cancellation-driven leakage  
2. **Double down on high-efficiency markets** such as the Netherlands, where retention and AOV are strongest  
3. **Rationalize low-performing inventory** using the Page 3 product quadrant analysis  

---

## 🎯 Why This Project Matters

- Demonstrates an end-to-end BI workflow from raw data to executive decisions  
- Focuses on *business outcomes*, not just visualization  
- Mirrors how retail analytics teams evaluate growth, efficiency, and risk  

---

## 📎 Tools Used
- Power BI  
- DAX  
- Time-series forecasting (exponential smoothing)  
- SQL-style data modeling concepts  

---

### 📖 Key Terminology
* **Net Revenue:** Gross sales minus cancellations/returns.
* **VIP Customer:** Top 10% of customers based on Frequency and Monetary value.
* **Revenue Leakage:** Potential revenue lost specifically to order cancellations.
* **April Anomaly:** A statistically significant spike in Home Decor cancellations identified in Q2 2011.

---

## 📌 Final Takeaway

This dashboard turns historical transaction data into a **cohesive growth narrative**.  
Rather than asking leaders to interpret charts, it answers the questions they actually care about:

**Where are we strong?  
Where are we leaking value?  
And where should we invest next?**
