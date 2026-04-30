# 📊 Vendor Performance Analysis

## 🧠 Project Summary
This project presents an end-to-end data analysis solution designed to evaluate vendor performance and optimize procurement strategies. By integrating multiple data sources and applying analytical techniques, the system provides actionable insights into vendor efficiency, profitability, and inventory utilization.

The solution is built with a pipeline-based architecture that transforms raw transactional data into a structured analytical model and delivers business-ready insights through an interactive dashboard.

---

## 🎯 Problem Statement
Organizations often face challenges in managing vendor-related decisions due to lack of visibility into:

- Vendor-wise profitability and cost efficiency  
- Inventory movement and stock utilization  
- Effectiveness of bulk purchasing strategies  
- Vendor dependency and associated risks  

Without structured analysis, these issues lead to poor procurement decisions, increased costs, and inefficient inventory management.

---

## 🏗️ Solution Architecture

The project follows a modular data pipeline approach:
```mermaid
flowchart LR
    A[Raw CSV Data] --> B[SQLite Database]
    B --> C[SQL Transformation using CTEs]
    C --> D[Feature Engineering]
    D --> E[EDA & Analysis]
    E --> F[Power BI Dashboard]

### 4️⃣ Exploratory Data Analysis (EDA)
*   Analyzed distribution of sales, costs, and margins.
*   Identified outliers and anomalies in vendor performance.
*   Evaluated vendor contribution to overall business revenue.
*   Compared purchasing vs selling trends.

### 5️⃣ Business Analysis
The project addresses critical business questions:
*   Which vendors generate high revenue but low profitability?
*   Which vendors contribute most to procurement costs?
*   Where is capital locked in unsold inventory?
*   Does bulk purchasing effectively reduce unit price?
*   What is the dependency on top-performing vendors?

### 6️⃣ Dashboard Development (Power BI)
Developed an interactive dashboard to support decision-making. Key features include **vendor performance ranking**, **profitability analysis**, and **inventory turnover insights**.

---

## 📈 Key Insights
*   **Pricing Inefficiencies:** Identified vendors with high sales but low profit margins.
*   **Inventory Management:** Detected slow-moving inventory leading to capital blockage.
*   **Procurement Strategy:** Found inconsistent benefits from bulk purchasing.
*   **Supply Chain Risk:** Highlighted vendor dependency risks.

## 💼 Business Impact
*   Optimize vendor selection and procurement strategy.
*   Reduce unnecessary costs and improve margins.
*   Enhance inventory management and turnover efficiency.
*   Make data-driven business decisions.

## ⚠️ Challenges Faced
*   Handling joins across multiple datasets without duplication.
*   Designing efficient SQL queries for large-scale aggregation.
*   Ensuring consistency between different data sources.
*   Translating raw data into meaningful business insights.

---

## 📁 Project Structure
```plaintext
├── data/                             # Raw datasets
├── ingestion_db.py                   # Data ingestion pipeline
├── get_vendor_summary.py             # SQL transformation & feature engineering
├── Exploratory Data Analysis.ipynb   # EDA notebook
├── Vendor Performance Analysis.ipynb # Analysis notebook
├── logs/                             # Log files
├── inventory.db                      # SQLite database
└── README.md
## Future Enhancements
*   **Workflow Orchestration:** Implement automated scheduling and monitoring using **Apache Airflow**.
*   **Real-time Processing:** Enable real-time or incremental data ingestion to keep insights current.
*   **Machine Learning:** Develop a **vendor scoring model** to predict and evaluate performance.
*   **Enterprise Deployment:** Deploy dashboards for scaled, enterprise-level access.

---

### 🧩 Key Learnings
*   **Pipeline Architecture:** Mastered end-to-end data pipeline design.
*   **Advanced SQL:** Utilized Complex **CTEs** and window functions for deep-dive analysis.
*   **Feature Engineering:** Created custom business metrics to drive strategy.
*   **Data Storytelling:** Successfully converted raw data into **actionable insights**.

---

### 👤 Author
**Tushar Parit**  
*Aspiring Data Analyst*  

**Skills:**  
`Python` | `SQL` | `Power BI`
  ### 4. 📉 Power BI Dashboard
 
![image](https://github.com/user-attachments/assets/07a32b68-783a-4a5a-abd8-19811b13974a)

![image](https://github.com/user-attachments/assets/ed666aa2-e286-442e-93f3-b567e1f03bf8)
