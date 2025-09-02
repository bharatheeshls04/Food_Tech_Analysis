# Food_Tech_Analysis
# 📊 A/B Test Analysis – Foodtech Hackathon Project

## 📌 Project Overview
This repository contains my submission for the **Compety Hackathon (March 2025)**.  
The task was to evaluate an **A/B test** run by a UK-based foodtech company to determine whether **larger food images on restaurant menu cards** lead to higher user conversion rates.  

The analysis includes:
- Evaluation of the A/B test design  
- Statistical testing of results  
- User behavior insights  
- Data-driven business recommendations  

---



## 📊 Dataset Overview
- Total events: **326,921**
- Key fields:
  - `variation`: 1 = Control (original UI), 2 = Test (larger images)  
  - `event_type`: reload_the_page, entry_to_shop, order_paid, order_finished  
  - `final_order_status`: Successful, Cancelled, Refunded  
  - `platform`: iOS / Android  

🔒 **Note:** The dataset provided in the hackathon is not publicly available due to competition rules.  
You can replicate the analysis using a similar dataset of user event logs.  

---

## ⚙️ Methodology
1. **Test Design Review**
   - Compared control (original UI) vs. test (larger images).  
   - Identified strengths and weaknesses (missing data, unclear randomization).  

2. **Exploratory Data Analysis (EDA)**
   - Cleaned missing values in `final_order_status` and `shop_id`.  
   - Segmented users by platform (iOS vs. Android).  

3. **Statistical Testing**
   - Conversion rate comparison between groups.  
   - Chi-Square test for independence.  

4. **Visualization**
   - Conversion rates by variation.  
   - Order status distribution.  
   - Platform-based performance.  

---

## 📈 Results
- **Conversion Rates:**  
  - Control: **42.41%**  
  - Test: **42.20%**  
  - No significant difference (**p-value = 0.5213**).  

- **Platform Insights:**  
  - Android users convert at ~28.9% vs. iOS users at ~13.5%.  
  - No significant difference between variations on either platform.  

- **Order Outcomes:**  
  - Majority of orders were successful.  
  - Minimal cancellations/refunds.  

---

## 💡 Business Recommendations
- Reconsider test variation — larger images did not improve conversions.  
- Investigate **why Android outperforms iOS** and replicate success.  
- Improve data quality (handle missing values in `final_order_status`).  
- Track more metrics (engagement, repeat purchases, session duration).  
- Run further A/B tests with different variations and longer test periods.  

---
## 📂 Repository Contents
AB_Test_Food_Tech_Analysis.ipynb # Detailed Python notebook with analysis

A-B_Test_Analysis_Presentation.pdf # Slide deck with insights & recommendations

README.md # Project overview
