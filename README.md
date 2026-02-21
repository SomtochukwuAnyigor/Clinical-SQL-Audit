# Advanced Clinical Audit: Population Health & Triage

## 📌 Project Overview
This project simulates a **Population Health Management** tool used to audit a large relational database of 100+ patients. It moves beyond basic querying to demonstrate how data analysts handle longitudinal records—identifying high-risk geriatric patients (Age 65+) with uncontrolled diabetes (HbA1c > 7.0) while filtering for the most recent clinical markers.

## 📊 Dashboard Summary
<img width="945" height="548" alt="Clinical Audit Summary" src="https://github.com/user-attachments/assets/fdd25f6c-2e43-4b89-b541-5a3524f479da" />

*Figure 1: Distribution of identified at-risk geriatric patients by priority level.*

## 🎯 Strategic Objectives
* **Scalability:** Managing and querying a database of 100 patients and 250+ lab records.
* **Longitudinal Analysis:** Using SQL aggregations to isolate the highest (worst-case) lab results per patient.
* **Risk Stratification:** Automating the triage process into "CRITICAL" and "HIGH RISK" categories.
* **Data Visualization:** Translating complex SQL outputs into an executive-level dashboard for hospital management.

## 🛠️ Tech Stack
* **Language:** SQL (SQLite)
* **Data Science:** Python (Pandas)
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Google Colab

## 🚀 Advanced SQL Features
* **Aggregate Functions:** Used `MAX()` and `COUNT()` within subqueries to handle patients with multiple lab entries.
* **Group By Logic:** Consolidated one-to-many relationships (one patient, many labs) into a single-row audit view.
* **CTEs (Common Table Expressions):** Modularized the high-risk filter for better performance.
* **Case Triage:** Categorized patients based on clinical thresholds (HbA1c >= 8.5 as Critical).



## 📂 How to Run
1. Open the notebook in **Google Colab**.
2. Run the **Power-Up Generator** cell to initialize the 100-patient clinical database.
3. Execute the **Advanced Audit Query** to view the prioritized patient list.
4. Run the **Visualization cell** to generate and download the Triage Distribution Chart.
