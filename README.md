# 🔁 Funnel Analysis – User Onboarding 

## 📌 Overview
This project conducts an **end-to-end funnel analysis** of a user onboarding journey, tracking users from **signup → email verification → KYC → first transaction**.  
The objective is to identify **conversion bottlenecks**, understand **behavior across funnel stages**, and generate **data-driven recommendations** to improve activation and transaction completion.

---

## 🎯 Business Objective
- Measure user progression across onboarding stages  
- Identify high-impact drop-off points  
- Evaluate conversion performance by **device** and **acquisition channel**  
- Surface actionable insights to improve funnel efficiency and ROI  

---

## 📂 Dataset
The analysis uses **user-level and event-level data**, including:
- Funnel timestamps (signup, email verification, KYC approval, transaction)
- Device type, country, app version
- Acquisition channel
- Event-level actions and system errors

---

## 🧹 Data Cleaning & Preparation (SQL)
All data preparation was performed in **SQL using a production-style workflow**:

- Created **staging tables** to preserve raw data integrity  
- Removed duplicate records using **window functions**  
- Standardized categorical fields (device, country, channel)  
- Normalized inconsistent app version values  
- Converted timestamps to `DATETIME` format  
- Handled null values and invalid event sequences  
- Removed extreme time-to-conversion outliers (>720 hours)

📂 **SQL Script:** `/sql/data_cleaning.sql`

---

## 🔍 Exploratory Data Analysis (EDA)
EDA was conducted entirely in SQL to quantify funnel performance and user behavior:

- Funnel-stage user counts  
- Stage-to-stage conversion rates  
- Drop-off analysis by stage  
- Conversion by device type and acquisition channel  
- Signup trends and time-to-conversion analysis  

📂 **SQL Script:** `/sql/eda.sql`

---

## 📊 Key Funnel Metrics
- **Signup → Transaction conversion:** ~**40%**  
- **Largest drop-off:** Post-KYC approval  
- **Highest-impact platforms:** Android & Web  
- **Insight:** High acquisition volume does not necessarily translate to high conversion quality  

---

## 📈 Tableau Dashboard
An interactive **Tableau dashboard** was built to enable stakeholder exploration and decision-making.

**Dashboard Features:**
- Funnel drop-off visualization  
- Conversion by device & acquisition channel  
- Signup trends over time  
- Parameter-driven filters for dynamic analysis  

🔗 **Tableau Dashboard:** *(Add link here)*

---

## 💡 Key Insights
- Post-KYC activation is the **primary conversion bottleneck**  
- Improving funnel efficiency delivers higher ROI than increasing acquisition volume  
- Android and Web platforms present the **fastest optimization opportunities**  
- Signup growth has plateaued, making funnel optimization business-critical  

---

## 🚀 Business Recommendations
- Improve post-KYC onboarding with **guided next steps and incentives**  
- Reduce friction during KYC initiation and approval handoff  
- Prioritize optimization efforts on **Android and Web**  
- Reallocate acquisition spend toward **high-conversion channels**  
- Re-engage KYC-approved but inactive users via targeted nudges  

---

## 🛠️ Tools & Technologies
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge)

- **SQL (MySQL)** – Data cleaning, EDA, and funnel metrics  
- **Tableau** – Interactive dashboarding and visualization  

---

## 👤 Author
**Dipanshi Dhiman**  
📊 Data Analyst | Canada  
Focused on product analytics, funnel optimization, and business insights
