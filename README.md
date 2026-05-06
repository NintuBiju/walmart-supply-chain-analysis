# 🛒 Walmart Supply Chain — Operational Efficiency Analysis

## Project Overview
This project analyses 500,000 supply chain events from Walmart's operations 
spanning 10 years (2016–2026). The goal is to identify where, when, and why 
operational delays and inefficiencies occur — and provide actionable 
recommendations for supply chain management.

This project was built to demonstrate a junior data analyst's end-to-end workflow:
from raw data exploration to insight generation.

---

## 🎯 Problem Statement
Walmart's supply chain handles millions of events daily — from supplier 
restocking and warehouse transfers to store deliveries and reverse logistics. 
Despite large volumes of data, it is unclear where operational delays are 
concentrated and what is driving them.

**Key questions this analysis answers:**
- What is the overall on-time delivery rate, and how does it vary by region and category?
- Which lifecycle stages experience the most delays?
- Are certain suppliers or carriers consistently associated with longer cycle times?
- Where do anomalies and exceptions cluster — and what are their root causes?

---

## 🗂️ Project Structure
walmart-supply-chain-analysis/
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_root_cause_analysis.ipynb
│   └── 05_insights_recommendations.ipynb
├── data/
│   └── data_description.md
└── images/

---

## 🛠️ Tools & Technologies
| Tool | Purpose |
|---|---|
| Databricks (Community Edition) | Notebook environment & cluster compute |
| Python (pandas, matplotlib, seaborn) | Data cleaning, analysis, visualisation |
| SQL | Aggregations and exploratory queries |
| GitHub | Version control and portfolio publishing |

---

## 📊 Dataset
- **Source:** Walmart Supply Chain synthetic dataset
- **Size:** 500,000 rows × 39 columns
- **Period:** January 2016 – January 2026
- **Key columns:** event_type, lifecycle_stage, on_time_flag, delay_days, 
  anomaly_flag, product_category, warehouse_region, supplier_name

See [`data/data_description.md`](data/data_description.md) for full details.

---

## 🔍 Key Findings
*(To be updated as analysis progresses)*

---

## 👤 Author
**Nintu**  
Aspiring Data Analyst  
[LinkedIn](#) | [GitHub](#)