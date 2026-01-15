\# Funnel Analysis Project (SQL + Tableau)

\# Funnel Analysis Project (SQL + Tableau)



\## 📌 Project Overview

This project presents an end-to-end \*\*funnel analysis of a user onboarding journey\*\*, tracking users from signup through first transaction. The goal was to identify conversion bottlenecks, analyze user behavior across funnel stages, and provide actionable, data-driven recommendations.



The project follows a real-world analytics workflow used in product and growth teams.



---



\## 🎯 Business Problem

High user acquisition does not translate into business value unless users successfully progress through key onboarding stages and complete transactions.



This analysis aims to:

\- Identify \*\*where users drop off\*\* in the onboarding funnel

\- Measure \*\*conversion rates\*\* at each stage

\- Analyze performance by \*\*device type\*\* and \*\*acquisition channel\*\*

\- Surface \*\*opportunities to improve first-transaction completion\*\*



---



\## 🗂 Dataset Overview

The project uses two primary datasets:



\### User-Level Data

\- Signup time

\- Email verification time

\- KYC started and approved times

\- First transaction time

\- Device type

\- Country

\- App version

\- Acquisition channel



\### Event-Level Data

\- Event name and order

\- Event timestamp

\- Device and country

\- KYC status and error reasons



Each user is tracked across the full onboarding funnel.



---



\## 🧹 Data Cleaning (SQL)

All data cleaning was performed in SQL to ensure data integrity before analysis.



Key steps included:

\- Creating \*\*staging tables\*\* to protect raw data

\- Removing \*\*duplicate records\*\* using `ROW\_NUMBER()` window functions

\- Standardizing categorical fields (device type, country, acquisition channel)

\- Normalizing app version values

\- Converting timestamp fields from text to `DATETIME`

\- Handling null and incomplete funnel stages

\- Removing extreme outliers (>720 hours) in time-to-conversion analysis



📂 SQL scripts available in the `/sql` folder.



---



\## 🔍 Exploratory Data Analysis (EDA)

EDA was conducted entirely in SQL to understand user behavior prior to visualization.



Key analyses:

\- Funnel stage user counts

\- Conversion and drop-off rates

\- Device-level conversion performance

\- Acquisition channel conversion quality

\- Monthly signup trends

\- Time-to-conversion between funnel stages

\- Event-level error analysis



---



\## 📊 Funnel Metrics Summary

\- Signup → Transaction conversion rate: \*\*~40%\*\*

\- Largest drop-off observed \*\*after KYC approval\*\*

\- Android and Web platforms dominate user activity

\- Acquisition volume does not always correlate with conversion quality



---



\## 📈 Tableau Dashboard

An interactive Tableau dashboard was built to visualize funnel performance and enable stakeholder exploration.



\*\*Dashboard includes:\*\*

\- Funnel visualization with stage-level drop-offs

\- Conversion by device type

\- Conversion by acquisition channel

\- Year-over-year signup trends

\- Parameter-driven filters for dynamic analysis



🔗 \*\*Tableau Public Link:\*\* \*(add your link here)\*  

📸 Dashboard screenshots available in the `/dashboard` folder.



---



\## 🔑 Key Insights

\- Post-KYC activation is the primary conversion bottleneck

\- Improving conversion efficiency has higher impact than increasing acquisition

\- Android and Web platforms offer the highest optimization leverage

\- Signup growth has plateaued, making funnel optimization critical



---



\## ✅ Recommendations

\- Improve post-KYC onboarding with guided next steps and incentives

\- Reduce friction during KYC initiation

\- Prioritize UX optimization on Android and Web

\- Shift acquisition spend toward high-conversion channels

\- Re-engage verified but inactive users through lifecycle campaigns



---



\## 🛠 Tools \& Technologies

\- \*\*SQL (MySQL)\*\* – Data cleaning, transformation, and EDA

\- \*\*Tableau\*\* – Interactive dashboard and visualization



---



\## 📂 Repository Structure



\## 📌 Project Overview

This project presents an end-to-end \*\*funnel analysis of a user onboarding journey\*\*, tracking users from signup through first transaction. The goal was to identify conversion bottlenecks, analyze user behavior across funnel stages, and provide actionable, data-driven recommendations.



The project follows a real-world analytics workflow used in product and growth teams.



---



\## 🎯 Business Problem

High user acquisition does not translate into business value unless users successfully progress through key onboarding stages and complete transactions.



This analysis aims to:

\- Identify \*\*where users drop off\*\* in the onboarding funnel

\- Measure \*\*conversion rates\*\* at each stage

\- Analyze performance by \*\*device type\*\* and \*\*acquisition channel\*\*

\- Surface \*\*opportunities to improve first-transaction completion\*\*



---



\## 🗂 Dataset Overview

The project uses two primary datasets:



\### User-Level Data

\- Signup time

\- Email verification time

\- KYC started and approved times

\- First transaction time

\- Device type

\- Country

\- App version

\- Acquisition channel



\### Event-Level Data

\- Event name and order

\- Event timestamp

\- Device and country

\- KYC status and error reasons



Each user is tracked across the full onboarding funnel.



---



\## 🧹 Data Cleaning (SQL)

All data cleaning was performed in SQL to ensure data integrity before analysis.



Key steps included:

\- Creating \*\*staging tables\*\* to protect raw data

\- Removing \*\*duplicate records\*\* using `ROW\_NUMBER()` window functions

\- Standardizing categorical fields (device type, country, acquisition channel)

\- Normalizing app version values

\- Converting timestamp fields from text to `DATETIME`

\- Handling null and incomplete funnel stages

\- Removing extreme outliers (>720 hours) in time-to-conversion analysis



📂 SQL scripts available in the `/sql` folder.



---



\## 🔍 Exploratory Data Analysis (EDA)

EDA was conducted entirely in SQL to understand user behavior prior to visualization.



Key analyses:

\- Funnel stage user counts

\- Conversion and drop-off rates

\- Device-level conversion performance

\- Acquisition channel conversion quality

\- Monthly signup trends

\- Time-to-conversion between funnel stages

\- Event-level error analysis



---



\## 📊 Funnel Metrics Summary

\- Signup → Transaction conversion rate: \*\*~40%\*\*

\- Largest drop-off observed \*\*after KYC approval\*\*

\- Android and Web platforms dominate user activity

\- Acquisition volume does not always correlate with conversion quality



---



\## 📈 Tableau Dashboard

An interactive Tableau dashboard was built to visualize funnel performance and enable stakeholder exploration.



\*\*Dashboard includes:\*\*

\- Funnel visualization with stage-level drop-offs

\- Conversion by device type

\- Conversion by acquisition channel

\- Year-over-year signup trends

\- Parameter-driven filters for dynamic analysis



🔗 \*\*Tableau Public Link:\*\* \*(add your link here)\*  

📸 Dashboard screenshots available in the `/dashboard` folder.



---



\## 🔑 Key Insights

\- Post-KYC activation is the primary conversion bottleneck

\- Improving conversion efficiency has higher impact than increasing acquisition

\- Android and Web platforms offer the highest optimization leverage

\- Signup growth has plateaued, making funnel optimization critical



---



\## ✅ Recommendations

\- Improve post-KYC onboarding with guided next steps and incentives

\- Reduce friction during KYC initiation

\- Prioritize UX optimization on Android and Web

\- Shift acquisition spend toward high-conversion channels

\- Re-engage verified but inactive users through lifecycle campaigns



---



\## 🛠 Tools \& Technologies

\- \*\*SQL (MySQL)\*\* – Data cleaning, transformation, and EDA

\- \*\*Tableau\*\* – Interactive dashboard and visualization



---



\## 📂 Repository Structure



