# 🛒 Olist E-Commerce Data Analytics Project

An end-to-end data analytics project exploring the Brazilian E-Commerce Public Dataset by Olist. This project uses SQL, Python, and Power BI to investigate sales performance, delivery efficiency, product categories, and data quality.

## 📌 1. Problem Statement

Olist is a Brazilian e-commerce marketplace that connects multiple sellers with customers across Brazil.

Understanding marketplace performance requires analyzing sales trends, order delivery performance, product categories, and customer activity.

The objective of this project is to:
- Analyze e-commerce sales and order trends.
- Identify delivery delays and operational issues.
- Examine product category performance.
- Evaluate data quality and missing information.
- Present actionable insights through an interactive Power BI dashboard.

## 📂 2. Dataset

**Source:** [Brazilian E-Commerce Public Dataset by Olist – Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The dataset contains approximately 100,000 orders placed between 2016 and 2018.

It consists of multiple interconnected CSV files, including:

| Dataset | Description |
|---|---|
| Orders | Order status and timestamps |
| Customers | Customer information and locations |
| Order Items | Products, prices, and sellers |
| Products | Product details and categories |
| Payments | Payment methods and installments |
| Reviews | Customer review scores |
| Sellers | Seller information |
| Geolocation | Brazilian ZIP code coordinates |

The datasets were cleaned, validated, and prepared for analysis before generating insights.

## 🔍 3. Key Findings

1. **Late Deliveries:** Approximately 7.87% of delivered orders were delivered later than their estimated delivery dates.

2. **Average Delivery Time:** The average delivery duration was approximately 12.09 days.

3. **Missing Product Categories:** 610 product records had missing category information, representing approximately 1.85% of product records.

4. **Missing Delivery Dates:** 2,965 orders had missing customer delivery timestamps, affecting delivery performance analysis.

5. **Geolocation Duplicates:** 261,831 duplicate records were identified in the geolocation dataset, highlighting the need for data quality checks before analysis.

*Note: Data-quality counts are identified during validation and should not be interpreted as business performance metrics.*

## 📊 4. Power BI Dashboard

The interactive Power BI dashboard provides an overview of marketplace performance through key performance indicators and visualizations.

Dashboard highlights:
- Sales and order performance.
- Monthly revenue trends.
- Product category analysis.
- Order and customer insights.
- Delivery performance.
- Customer review analysis.

![Olist Power BI Dashboard](screenshots/dashboard.png)

## 🛠️ 5. Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data cleaning and exploratory analysis |
| Pandas & NumPy | Data manipulation and processing |
| Matplotlib | Data visualization |
| MySQL | Database management and SQL analysis |
| Power BI | Interactive dashboards and reporting |
| DAX | Calculated measures and KPIs |
| Jupyter Notebook | Python analysis environment |
| Git & GitHub | Version control and project hosting |

## 📁 6. Project Structure

```text
Olist-Data-Analytics/
│
├── python/
│   └── olist_analysis.ipynb
│
├── sql/
│   └── olist_analysis.sql
│
├── powerbi/
│   └── Olist_Dashboard.pbix
│
├── screenshots/
│   └── dashboard.png
│
└── README.md
```

## 🚀 7. How to Run

### Prerequisites
- Python 3.x
- Jupyter Notebook
- MySQL
- Power BI Desktop

### Step 1: Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Olist-Data-Analytics
```

### Step 2: Set up Python

```bash
python -m venv venv
```

Activate the environment:

**Windows:**
```bash
venv\Scripts\activate
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib jupyter
```

### Step 3: Prepare the dataset

1. Download the Olist dataset from Kaggle.
2. Extract the CSV files.
3. Place the dataset files in the appropriate project data folder.
4. Configure your local database connection if required.

### Step 4: Run SQL analysis

1. Open MySQL Workbench.
2. Create the project database.
3. Import the required CSV datasets.
4. Open and execute the SQL scripts in the `sql/` folder.

### Step 5: Run Python analysis

```bash
jupyter notebook
```

Open `olist_analysis.ipynb` and execute the notebook cells.

### Step 6: Open the Power BI dashboard

1. Open Power BI Desktop.
2. Open `powerbi/Olist_Dashboard.pbix`.
3. Update the data source paths if necessary.
4. Refresh the data to view the dashboard.

---

**Project Focus:** Data Cleaning | SQL Analysis | Exploratory Data Analysis | Business Insights | Power BI Visualization
