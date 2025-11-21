## **Project Description**

This project explores the financial performance of **S&P 500 companies** using a fully reproducible Python-based analytics workflow. The goal is to transform raw fundamental data into meaningful insights about **profitability, cost structure, growth dynamics, and competitive positioning**.

The analysis combines traditional financial metrics with data science techniques such as **clustering, forecasting, and ratio modeling**, offering a holistic view of firm performance beyond simple revenue comparisons.

The project follows a structured approach:

---

## **1. Data Cleaning & Feature Engineering**

The raw Kaggle dataset contains quarterly data for **2,012 financial observations** across **multiple S&P 500 firms**.
A robust cleaning pipeline was constructed:

* Parsing and standardizing date fields
* Sorting financial statements chronologically
* Generating yearly aggregations
* Engineering profitability ratios:

  * Gross Margin
  * Operating Margin
  * Net Margin
  * R&D Ratio
  * SG&A Ratio

These ratios allow **cross-company comparisons independent of size**, building the foundation for deeper analytics.


## **2. Firm-Level Financial Summary**

Each firm is summarized using multi-year averages:

* Average Revenue
* Average Net Income
* Margin Structure
* Cost ratios (R&D, SG&A relative to revenue)

This transforms fragmented quarterly data into high-level company profiles—similar to what an analyst or consultant would prepare for benchmarking or due diligence.


## **3. Revenue & Profitability Trend Analysis**

Time-series functions calculate:

* Annual Revenue
* Annual Net Income
* Revenue and Net Income in billions
* Year-over-Year (YoY) changes

This trend view highlights how each company evolves over time, revealing:

* Growth slowdowns
* Margin cycles
* Periods of volatility
* Shifts in operational performance

Example:
Amazon’s 2021 revenue growth slowed to **–0.046%**, while net income jumped **+17.21%**, showing higher bottom-line efficiency despite flat top-line performance.


## **4. Margin Structure Analysis**

The project evaluates how efficiently companies turn revenue into profit:

* Gross Margin → product-level efficiency
* Operating Margin → operating cost discipline
* Net Margin → ultimate profitability after non-operating items

Margins are converted into percentages for intuitive interpretation.

This enables high-level questions such as:

* Is a company high-margin or volume-driven?
* Is profitability improving or deteriorating?
* How does a company’s cost structure compare to peers?


## **5. Peer Comparison (Industry Benchmarking)**

A dedicated function compares **AMZN, COST, TGT, and WMT** in a chosen year (2021).
Metrics include:

* Total Revenue
* Net Income
* Gross Margin %
* Operating Margin %
* Net Margin %

This supports insights such as:

* Costco and Walmart operate on extremely thin margins
* Target’s profitability profile is closer to Amazon than big-box peers
* Revenue scale alone does not determine earnings power

This mirrors how analysts build competitive benchmarking slides.


## **6. Profitability-Based Clustering (K-Means)**

To uncover structural patterns across the S&P 500, k-means clustering is applied using firm-level ratios.

The clustering reveals groups of companies based on:

* Capital-light vs capital-heavy models
* R&D-intensive vs low-R&D firms
* High-margin vs low-margin performance
* SG&A spending intensity

This dimensionality reduction transforms hundreds of financial lines into **strategic profitability archetypes**.


## **7. Forecasting Future Revenue**

Two forecasting methods are implemented:

### **Linear Regression**

Projects revenue assuming a stable linear trend, producing a clean quarterly forward projection.

### **ARIMA Model**

Captures time-series dynamics and provides:
* Point forecast
* 95% lower bound
* 95% upper bound

This mirrors forecasting workflows used in finance, corporate planning, and consulting.

---

## 👩🏻‍💻 About Me

**Ayu Putri Vidiantiwi**  
* 📚 M.S. in Applied Analytics, Columbia University  
* 📊 Passionate about finance, business, data storytelling, and analytics
* 🌐 LinkedIn - https://www.linkedin.com/in/ayuputriv/
* 📧 ayu.vidiantiwi@columbia.edu
