# 📦 Inventory & Vendor Performance Analysis – Manufacturing Case Study

An end-to-end analytics pipeline built on a realistic manufacturing case study to optimize inventory management and vendor performance. This project demonstrates industry-standard best practices for data ingestion, transformation, statistical analysis, and business intelligence using anonymized transactional data.

---

## 📖 Overview

* **Domain:** Medium-sized manufacturing company producing electronic components
* **Data Scale:** Multi-million-row CSV files for purchases, sales, inventory, and vendor invoices
* **Objective:** Identify inefficiencies in stock levels, reduce carrying costs, and enhance vendor management
* **Confidentiality:** Actual product and brand names replaced with generic placeholders (e.g., “Product A”, “Product B”)

---

## 🚀 Key Features

1. **Data Ingestion & Audit Logging**
   Python scripts ingest raw CSV data into a SQL database with detailed log capture (`logs/ingestion_db.log`).

2. **Data Transformation & Modeling**
   SQL and Python collaboratively generate a clean, vendor-level summary table from transactional records.

3. **Advanced Analytics & Hypothesis Testing**
   Jupyter Notebooks perform feature engineering, exploratory data analysis (EDA), and rigorous statistical tests to uncover insights on profit margin, stock turnover, and unsold inventory.

4. **Interactive Business Intelligence**
   A Power BI dashboard visualizes key performance indicators (KPIs) such as profit margins, stock-to-sales ratios, and reorder recommendations.

5. **Modular & Reproducible Workflow**
   Clear folder structure and configuration enable seamless onboarding for new analysts and easy pipeline maintenance.

---

## 📂 Project Structure

```
inventory-vendor-analysis/
│
├── data/                       # (Optional) Sample or small CSV files
│
├── ingestion/                  # Data loading scripts and configuration
│   └── ingest_to_db.py         # CSV → SQL ingestion logic with logging
│
├── notebooks/                  # Jupyter notebooks for analysis and modeling
│   ├── 01_create_summary_table.ipynb  # Summary table generation (SQL + Python)
│   └── 02_analysis_eda.ipynb         # EDA, feature engineering, hypothesis testing
│
├── dashboard/                  # Business intelligence and reporting
│   └── InventoryDashboard.pbix # Power BI dashboard
│
├── logs/                       # Log files for auditing and debugging
│   └── ingestion_db.log        # Timestamps and process logs for ingestion
│
├── docs/                       # Supporting documentation
│   └── data_dictionary.md      # Detailed schema and column definitions
│
├── .gitignore                  # Specifies files and folders to ignore in Git
├── LICENSE                     # Project license (MIT)
├── README.md                   # Project overview and instructions
└── requirements.txt            # Python dependencies
```

---

## 🛠️ Technologies & Dependencies

* **Python 3.x**: `pandas`, `SQLAlchemy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`
* **SQL**: PostgreSQL (or SQLite) for data storage and aggregation
* **Jupyter Notebook**: Interactive data exploration and analysis
* **Power BI**: Interactive dashboard and reporting
* **Logging**: Python `logging` module for ETL audit trails

See `requirements.txt` for exact package versions.

---

## 🔧 Setup & Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/inventory-vendor-analysis.git
   cd inventory-vendor-analysis
   ```

2. **Create a virtual environment & install dependencies**

   ```bash
   python -m venv venv
   source venv/bin/activate      # macOS/Linux
   venv\Scripts\activate       # Windows
   pip install -r requirements.txt
   ```

3. **Configure database connection**
   Edit the database credentials in `ingestion/ingest_to_db.py` or set environment variables (`DB_HOST`, `DB_NAME`, `DB_USER`, `DB_PASS`).

4. **Ingest raw data**

   ```bash
   python ingestion/ingest_to_db.py
   ```

5. **Run Jupyter Notebooks**

   ```bash
   jupyter lab
   ```

   * Open `01_create_summary_table.ipynb` to build the summary table
   * Open `02_analysis_eda.ipynb` for analysis and hypothesis testing

6. **Open Power BI Dashboard**
   Launch Power BI Desktop and open `dashboard/InventoryDashboard.pbix`.

---

## 📚 Data Documentation

For a detailed schema and column definitions of all source and summary tables, see:

* `docs/data_dictionary.md`

---

## 📊 Dashboard Preview

*(Include a screenshot or GIF of your Power BI dashboard here. Save it under `dashboard/images/` and reference with Markdown.)*

```markdown
![Dashboard Preview](dashboard/images/dashboard_preview.png)
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ Contact & Contribution

**Saif Shaikh**

> Email: [youremail@example.com](mailto:youremail@example.com)
> LinkedIn: [linkedin.com/in/yourprofile](https://www.linkedin.com/in/yourprofile)

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or issue on GitHub.
