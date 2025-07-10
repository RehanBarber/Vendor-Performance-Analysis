# 📦 Inventory & Vendor Performance Analysis

An end-to-end analytics pipeline built for a growing manufacturing business managing diverse product lines. This personal portfolio project demonstrates industry‑standard best practices in data ingestion, transformation, statistical analysis, and interactive dashboarding using anonymized transactional data.

> 📌 This is a personal portfolio project intended for demonstration purposes only.

---

## 📖 Overview

* **Domain:** Manufacturing company handling general products
* **Data Scope:** Multi‑million‑row CSV files for inventory, purchases, sales, and vendor invoices
* **Objective:**

  * Identify stock inefficiencies
  * Reduce carrying costs
  * Enhance vendor management

---

## 🚀 Key Features

1. **📥 Data Ingestion & Audit Logging**

   * Ingestion/ingestion\_db.py loads raw CSV files into a SQL database
   * Detailed logs captured in Logs/ingestion\_db.log for full traceability

2. **🔄 Data Transformation & Modeling**

   * Combined SQL and Python workflows generate a clean, vendor‑level summary table

3. **📊 Advanced Analytics & Statistical Testing**

   * Jupyter notebooks perform EDA, feature engineering, and hypothesis testing on profit margins, stock turnover, and unsold inventory

4. **📈 Interactive Dashboarding**

   * Power BI report visualizes KPIs such as profit margins, stock‑to‑sales ratios, and reorder recommendations
   * Includes dynamic charts, tables, and KPI cards

5. **🗂️ Modular, Scalable Structure**

   * Clear separation of images, ingestion scripts, logs, and analysis notebooks
   * Easy onboarding for new collaborators or future extensions

---

## 📁 Project Structure

Dashboard/
├── images/
│   ├── Dashboard\_preview\.png        # Power BI dashboard snapshot
│   └── Vendor PerformanceDashboard.pbix  # Interactive Power BI file

├── Ingestion/
│   └── ingestion\_db.py              # Script for loading raw data into DB

├── Logs/
│   └── ingestion\_db.log             # ETL process logs

├── Notebooks/
│   ├── Vendor Performance Analysis.ipynb        # Main EDA & insights
│   └── Vendor Performance Analysis (Transformed).ipynb  # Data Transformation & summary table

├── .gitignore                       # Files/folders ignored by Git
├── README.md                        # Project documentation (this file)
└── requirements.txt                 # Python dependencies

---

## 🛠️ Tech Stack & Dependencies

* **Python 3.x:** pandas, numpy, SQLAlchemy, matplotlib, seaborn, scipy, statsmodels
* **SQL:** PostgreSQL or SQLite
* **Jupyter Notebook:** Interactive data exploration
* **Power BI:** Dashboard creation & reporting
* **Logging:** Built‑in Python logging module

Refer to requirements.txt for exact package versions.

---

## ⚙️ Setup & Installation

1. **Clone the repository**
   git clone [https://github.com/Saif907/vendor-performance-dashboard.git](https://github.com/Saif907/vendor-performance-dashboard.git)
   cd vendor-performance-dashboard

2. **Create & activate a virtual environment**
   python -m venv venv
   source venv/bin/activate      # macOS/Linux
   venv\Scripts\activate         # Windows

3. **Install dependencies**
   pip install -r requirements.txt

4. **Load raw data into the database**
   python Ingestion/ingestion\_db.py

5. **Explore analysis notebooks**
   jupyter lab

   * Vendor Performance Analysis.ipynb → EDA & insights
   * Vendor Performance Analysis (Transformed).ipynb → Data transformation & summary table

6. **View the Power BI dashboard**
   Open Power BI Desktop and load Dashboard/Vendor PerformanceDashboard.pbix

---

## 📊 Dashboard Preview

![Dashboard Preview](images/Dashboard_preview.png)

---

## 🙋 Contact

**Saif Shaikh**
📧 saif81868@gmail.com
🔗 www.linkedin.com/in/saif-shaikh-527346251

Feel free to explore the code and reach out with any questions or feedback!
