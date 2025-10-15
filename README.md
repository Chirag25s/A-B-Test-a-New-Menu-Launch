# A/B Test a New Menu Launch — Predictive Analytics Project

## Project Overview
I conducted an **A/B test analysis** for **Round Roasters**, a premium coffee chain in the U.S., to determine whether introducing a **new gourmet menu** and launching a **TV advertising campaign** could generate enough incremental profit to justify a significant increase in marketing costs.

The goal was to analyze transaction data from the test period and control stores, identify whether the new menu resulted in a statistically significant increase in profit, and recommend whether the new menu should be rolled out to all stores.

---

## My Methodology

### Step 1: Planning the Analysis
Before diving into data cleaning, I defined a clear analytical plan:
- **Performance metric:** `gross_margin` (used to measure profit growth)
- **Test period:** `2016-04-29` to `2016-07-21`  
  *(compared to the same 12-week period in 2015)*
- **Level of aggregation:** Weekly transaction data per store

This planning ensured a structured approach to data preparation and test design.

---

### Step 2: Data Preparation and Cleaning
I worked with three key datasets:
1. `round-roaster-stores.csv` – Store-level information for all locations  
2. `treatment-stores.csv` – Details of 10 stores (5 in Denver, 5 in Chicago) that tested the new menu  
3. `round-roaster-transactions.zip` – Transaction-level data for all stores (Jan 2015 – Aug 2016)

**Actions performed:**
- Filtered data for the relevant test and comparison periods  
- Aggregated transactions to the **weekly level per store**  
- Verified consistency across store IDs and time ranges  
- Ensured no duplicates or missing values in the final dataset

---

### Step 3: Matching Treatment and Control Units
To ensure a fair A/B comparison, I matched **two control stores** for each treatment store from the same region.

**Steps:**
- Created **trend** and **seasonality** features using 12-week rolling averages  
- Analyzed potential **control variables** from the store dataset (e.g., region, store size, average transactions, average sales)
- Calculated a **correlation matrix** between these variables and the performance metric (`gross_margin`)  
- Selected the most correlated variables for matching

This matching process helped minimize bias and control for regional and seasonal differences between test and control stores.

---

### Step 4: A/B Test Analysis
Once the matching was complete, I compared performance metrics between the treatment and control groups during the test period.

**Analytical approach:**
- Calculated **weekly average gross margins** for both groups  
- Measured **incremental lift** in profit for treatment stores relative to controls  
- Used **statistical testing** to validate whether observed differences were significant  
- Interpreted the business implications of the results

---

### Step 5: Insights and Recommendations
After analyzing the results:
- Evaluated whether the **profit growth exceeded the 18% threshold** required to justify the marketing investment  
- Summarized findings into a concise **report and business recommendation**

This step translated statistical findings into **actionable business insights** for management decision-making.

---

## Skills Demonstrated
- Data preparation and feature engineering  
- Experimental design and A/B testing methodology  
- Correlation analysis and control variable selection  
- Statistical interpretation and business insight generation  
- Data-driven storytelling and communication

---

## Data Sources

All datasets used in this project are available in the shared Google Drive folder below:

📁 **[Access All Data Files Here](https://drive.google.com/drive/folders/1X6J7GcvTSQ5egC7Wkabdii9jLkGz7m3F?usp=sharing)**

| File Name | Description |
|------------|-------------|
| `round-roaster-stores.csv` | Store information for all Round Roaster locations |
| `treatment-stores.csv` | Test stores that implemented the new menu |
| `round-roaster-transactions.zip` | Transaction-level data for all stores from Jan 2015 to Aug 2016 |

---

## Results Summary
- The analysis evaluated whether the **new menu and TV campaign** led to a significant **increase in profit growth**.
- The results were presented in a detailed report outlining the **incremental lift**, **statistical findings**, and **business recommendation** for management.

> 📄 *The complete A/B test analysis report and findings can be found in this repository.*

---

## Tools & Technologies
- **Python** (Pandas, NumPy, StatsModels, Matplotlib)
- **Alteryx** for data pipeline
- **Excel / Google Sheets** for validation
- **Power BI** for visualization and storytelling
- **Statistical Methods:** Correlation matrix, A/B test design, matching, hypothesis testing

---

## Conclusion
This project demonstrated my ability to:
- Design and execute an **A/B testing framework**  
- Derive actionable business insights from experimental data  
- Translate statistical evidence into **strategic recommendations**

It showcases my **end-to-end data analytics process** — from defining the problem to presenting a decision-oriented result.

---

## Final Deliverables
- Cleaned and aggregated dataset  
- A/B matching analysis notebook  
- Statistical results summary  
- Final report with business recommendations
