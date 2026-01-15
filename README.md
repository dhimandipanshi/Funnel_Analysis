# Funnel Analysis Project (SQL & Tableau)

## Overview
This project performs an end-to-end **funnel analysis of a user onboarding journey**, tracking users from signup to first transaction. The goal is to identify conversion bottlenecks, understand user behavior across funnel stages, and recommend data-driven improvements to increase transaction completion.

---

## Business Objective
- Measure user progression through onboarding stages
- Identify high-impact drop-off points
- Evaluate conversion performance by device and acquisition channel
- Surface actionable insights to improve funnel efficiency

---

## Dataset
The analysis uses user-level and event-level data containing:
- Funnel timestamps (signup, email verification, KYC, transaction)
- Device type, country, app version
- Acquisition channel
- Event-level actions and errors

---

## Data Cleaning (SQL)
All preparation was performed in SQL using a production-style workflow:
- Created staging tables to preserve raw data
- Removed duplicate records using window functions
- Standardized categorical fields (device, country, channel)
- Normalized app version values
- Converted timestamps to `DATETIME`
- Handled nulls and invalid sequences
- Removed extreme time-to-conversion outliers (>720 hrs)

📂 See `/sql/data_cleaning.sql`

---

## Exploratory Data Analysis (EDA)
EDA was conducted in SQL to quantify funnel performance:
- Funnel stage user counts
- Stage-to-stage conversion rates
- Drop-off analysis
- Device and acquisition channel conversion
- Signup trends and time-to-conversion

📂 See `/sql/eda.sql`

---

## Funnel Metrics (Key Results)
- Signup → Transaction conversion: **~40%**
- Largest drop-off: **Post-KYC approval**
- Highest-impact platforms: **Android & Web**
- Acquisition volume ≠ conversion quality

---

## Tableau Dashboard
An interactive Tableau dashboard visualizes funnel performance and enables stakeholder exploration.

**Includes:**
- Funnel drop-offs
- Conversion by device & channel
- Signup trends over time
- Parameter-driven filters

🔗 **Tableau Dashboard **

## Key Insights
- Post-KYC activation is the primary conversion bottleneck
- Improving conversion efficiency has higher ROI than increasing acquisition
- Android and Web offer the fastest optimization wins
- Signup growth has plateaued, increasing the importance of funnel optimization

---

## Recommendations
- Improve post-KYC onboarding with guided next steps and incentives
- Reduce friction during KYC initiation
- Prioritize optimization on Android and Web
- Reallocate acquisition spend toward high-conversion channels
- Re-engage verified but inactive users

---

## Tools
- **SQL (MySQL)** – Data cleaning & EDA  
- **Tableau** – Visualization & dashboarding

---

## Author
**Dipanshi Dhiman**  
Data Analyst | Canada
