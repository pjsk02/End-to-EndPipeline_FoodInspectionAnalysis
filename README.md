# 🏙️ Food Inspections Data Warehouse Project  
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

---

## Dimensional Model
![Dimensional Model Overview](./assets/DimensionalModel.png)
---

## 📊 Power BI Dashboard  

Built an interactive BI report with:  
- 📆 Temporal trends in inspections  
- 🏚️ High-risk restaurant identification  
- ⚠️ Violation frequency analysis  
- 🌍 Geographical heatmaps of inspection results  

> 🔗 _Sample screenshots can be added here if you're sharing publicly_

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
**Feel free to fork, explore, and contribute!**
📬 Let’s connect on [LinkedIn](https://www.linkedin.com/in/je-pulipati/) If you’re hiring for Data Engineering, Analytics, or BI intern roles im open hiring!

---
