# 🦄 The Global Unicorn Landscape (2019–2022): A PostgreSQL Analysis

[![SQL](https://img.shields.io/badge/SQL-PostgreSQL-blue.svg)](https://www.postgresql.org/)
[![Environment](https://img.shields.io/badge/Environment-Jupyter_Notebook-orange.svg)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

## 📌 Project Overview
A "unicorn" is a privately held startup company with a valuation of over $1 billion. This project provides a comprehensive data-driven exploration of the global unicorn landscape during one of the most volatile periods in modern financial history: the steady growth of 2019–2020, the unprecedented venture capital boom of 2021, and the severe market correction of 2022. 

The primary objective of this project is to use advanced SQL techniques to extract actionable business intelligence regarding industry velocity, investor influence, geographic growth trends, and capital efficiency.

## 🗄️ Database Schema
The analysis is built on a relational database containing over 1,000 unicorn companies globally, structured across four key tables:
* **`companies`**: Geographic footprint (country, continent, city) of each startup.
* **`industries`**: Market sector categorization (e.g., Fintech, Edtech, SaaS).
* **`dates`**: Timeline tracking from the year founded to the exact date of reaching unicorn status.
* **`funding`**: Financial metrics, including total funding raised, current valuation, and key venture capital investors.

## 📊 Key Business Questions & Insights

### 1. Industry Velocity
* **Question:** Which industries reach unicorn status the fastest?
* **Insight:** Physical-world sectors like Auto & Transportation (4 years) scale faster to $1B valuations than strictly digital sectors like Internet Software (7 years), highlighting the impact of heavy capital investments in physical tech.

### 2. Investor Portfolio Valuation
* **Question:** Who are the most prolific investors, and what is the total combined valuation of all the unicorns they have backed?
* **Insight:** While Accel backed the highest volume of companies (60), Sequoia Capital China dominates the total value metric, backing 48 companies with a staggering combined valuation of $473 Billion.

### 3. Emerging Hubs & YoY Growth (2020–2022)
* **Question:** Which countries were the fastest-growing emerging hubs during the 2021 bubble, and who survived the 2022 crash?
* **Insight:** 2021 saw massive global inflation in unicorn minting (e.g., Canada growing by 1,400%). The 2022 market correction caused a universal drop in volume, though resilient markets like India and France successfully retained higher baselines than their pre-bubble numbers.

### 4. Capital Efficiency 
* **Question:** Which companies generated the highest valuations while taking the least amount of venture capital?
* **Insight:** Companies like Zapier (4,000:1 ratio) prove that extreme bootstrapping can result in massive enterprise value without dilutive venture capital. Furthermore, software isn't the only efficient sector; hardware manufacturers like DJI Innovations also rank in the global Top 10 for capital efficiency.

## 🛠️ Technical Skills & SQL Concepts Demonstrated
* **Relational Database Management:** Advanced `INNER JOIN` operations to unify complex schemas.
* **String Manipulation:** Cleaning and expanding comma-separated lists using `STRING_TO_ARRAY()` and `UNNEST()`.
* **Time-Series Analysis:** Safely calculating Year-over-Year (YoY) growth using `LAG()` and `COUNT() OVER()` window functions isolated by geographic partitions.
* **Data Reshaping:** Pivoting vertical time-series data into horizontal, dashboard-ready columns using `CASE WHEN` and `MAX()` aggregations.
* **Mathematical & Statistical Aggregation:** Calculating exact medians and quartiles using `PERCENTILE_CONT()`, while managing SQL type constraints and integer division.
* **Conditional Business Logic:** Deploying nested `CASE` statements to programmatically categorize numerical ratios into qualitative business tiers.
* **Query Optimization:** Structuring highly complex queries using modular Common Table Expressions (CTEs) for readable, maintainable production-level code.

## 🚀 How to View the Project
1. Open the [Jupyter Notebook](link-to-your-notebook.ipynb) to view the complete SQL code, table outputs, and in-depth business analysis.
2. The raw dataset (if applicable/allowed) is located in the `data/` folder.

---
*Created by [Your Name] - Connect with me on [LinkedIn](Link) or view my other projects on [GitHub](Link).*
