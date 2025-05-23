# 🏙️ Food Inspections Data Warehouse Project  

### Dashboard Link : https://app.powerbi.com/groups/me/reports/2b0f49c5-e2d0-4b6c-afe1-128b4303dc6f/7638e95db92838a5585c?experience=power-bi

---
## 📌 Summary  

🚀 **End-to-End Data Pipeline & BI Project** using real-world food inspection datasets from **Chicago** and **Dallas**.  
This project demonstrates my capabilities in:  

✅ **Data Engineering** – ETL pipeline design, cloud data warehouse modeling, data transformation  
✅ **Data Analytics** – profiling, cleansing, parsing, risk scoring, and deriving actionable metrics  
✅ **Business Intelligence** – storytelling with Power BI dashboards for inspection trends and violations  

---

## 📂 Datasets  

### 🍕 Chicago Food Inspections  
- ~290,000 records | 17 columns  
- Columns: Inspection ID, Establishment Info, Violations, Risk Level, Geo-coordinates  

### 🍔 Dallas Food Inspections  
- ~79,000 records | 114 columns  
- Columns: Address Details, Violation Set (up to 25 per row), Inspection Score  

---

## 🛠️ Tech Stack  
| Category               | Tools Used                                                                 |
|------------------------|----------------------------------------------------------------------------|
| Data Profiling         | `YData`, `Alteryx`                                                         |
| ETL & Pipeline         | `Azure Data Factory`, `Snowflake`, `Databricks`, `SQL`                     |
| Data Modeling          | `ER/Studio` – Dimensional Schema (Star Schema)                            |
| Data Visualization     | `Power BI` – KPI Dashboards, Interactive Filters                          |
| Scripting & Cleaning   | `Python`, `Regex`, `SQL`                                                  |

---

## 🧼 Data Engineering Process  

### 🧱 Medallion Architecture  
Implemented the **Bronze → Silver → Gold** architecture using Snowflake & Azure ADF.  

- **Bronze**: Raw ingestion via SnowSQL  
- **Silver**: Data cleaning & staging in Databricks  
- **Gold**: Star schema modeling in Snowflake using ADF pipelines  

---

### 🔄 ETL Highlights  

#### Dallas Dataset  
- Cleaned 114-column wide data using **Alteryx workflows**
- Parsed nested violation fields (pipe + comma separated)  
- Derived **Inspection Result**, **Risk Level**, **Total Violation Score**  
- Used REGEX to standardize names, split columns, remove whitespace  
- Merged 25 separate violation columns into normalized rows  

#### Chicago Dataset  
- Deduplicated based on `Inspection ID`  
- Flattened violation records (1 row per violation)  
- Formatted ZIP, City names, Risk Level values  
- Standardized column headers and cleaned residual whitespace  

---

## 🧾 Data Warehouse Design  

🧠 **Grain**: One row per violation per restaurant per inspection date  

### 📌 Dimension Tables  
- `DIM_LOCATION`, `DIM_INSPECTION`, `DIM_RESTAURANT`, `DIM_RESULT`, `DIM_RISK`, `DIM_VIOLATION`

### 📌 Fact Table  
- `FACT_INSPECTION` – captures each violation and joins all dimension keys  

✅ All tables created and loaded via **Azure Data Factory pipelines**

---
## 📈 Key Skills Demonstrated  

- ⛓️ End-to-End Data Pipeline Creation  
- 🗄️ Dimensional Modeling & Data Warehouse Development  
- 🧹 Advanced Data Cleaning (Regex, Parsing, Reshaping)  
- 🔁 ETL Orchestration using **Azure Data Factory**  
- 📊 KPI Dashboarding in **Power BI**  

---

## 🎯 What This Project Proves  

✔️ My ability to manage real-world messy data and convert it into structured, insightful assets  
✔️ End-to-end ownership of **data engineering** and **analytics pipeline**  
✔️ Strong grasp of **BI tools**, **SQL**, **ETL**, and **cloud data platforms**

---

## Dimensional Model

![DimensionalModel](https://github.com/user-attachments/assets/76a07d40-1e9f-4a73-a0d6-7d53d939a6af)

---

## Pipeline (Azure Data Factory)

![DataPipeline](https://github.com/user-attachments/assets/46c88787-82a2-4c80-9733-c79720b0c662)

---

## 📊 Power BI Dashboard  

Built an interactive BI report with:  
- 📆 Temporal trends in inspections  
- 🏚️ High-risk restaurant identification  
- ⚠️ Violation frequency analysis  
- 🌍 Geographical heatmaps of inspection results  

![Dashboard_HomeScreen](https://github.com/user-attachments/assets/1d825e36-3544-4a53-a531-8ddf22571ca4)

![Dashboard_P1_InspectionSumary](https://github.com/user-attachments/assets/f55ef30e-8c44-4434-b2cc-542f4944fbda)

![Dashboard_P2_FcilityType_RiskAnalysis](https://github.com/user-attachments/assets/501f3ee3-7f76-40d9-bf45-9904b08b136c)

![Dashboard_P3_RiskAnalysis](https://github.com/user-attachments/assets/0a8ef768-42df-4bc2-bbb3-688e9c237af6)

![Dashboard_P4_LocationInsights](https://github.com/user-attachments/assets/ee406600-70b2-43e6-81b6-1bea6d1400bc)

![Dashboard_P5_TopViolatoins](https://github.com/user-attachments/assets/c776c17f-df97-4c22-b42c-9c39470c362d)

![Dashboard_P6_AIPowered_BusinessInsights](https://github.com/user-attachments/assets/abaed663-822d-4b25-972b-93ff0895fcb8)

![Dashboard_P7_BusinessInsightsReport](https://github.com/user-attachments/assets/287fc845-5159-42d4-bd43-807256a8c037)

---

**Feel free to fork, explore, and contribute!**
📬 Let’s connect on [LinkedIn](https://www.linkedin.com/in/je-pulipati/) If you’re hiring for Data Engineering, Analytics, or BI intern roles im open hiring!

---
