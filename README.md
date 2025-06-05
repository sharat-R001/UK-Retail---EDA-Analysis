# 🛒 Online Retail Data Analysis (RFM & EDA)

This project performs in-depth data analysis on a UK-based e-commerce dataset, covering cleaning, feature engineering, exploratory analysis, visualizations, and **RFM segmentation** for customer profiling.

---

## 📦 Dataset

- Source: `Online Retail.xlsx`
- Transactions of a UK-based online retail store from 2010–2011
- Key columns: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🔍 Workflow Breakdown

### 1. 📥 Data Loading & Cleaning
- Loaded data using `pandas.read_excel()`
- Removed:
  - Rows with missing `CustomerID`
  - Canceled transactions (`InvoiceNo` starting with 'C')
- Handled incorrect/invalid entries
- Created `TotalSales = Quantity × UnitPrice`

### 2. 📊 Exploratory Data Analysis (EDA)
- Shape and structure of the dataset
- Frequency analysis for `StockCode` and `Description`
- Monthly transaction patterns

### 3. 📈 Visualization
- **Line plot** for monthly sales trend
- **Bar chart** for top 5 countries by revenue
- Grid layouts for better clarity

### 4. 🎯 RFM Analysis
Calculated:
- **Recency** – Days since last purchase
- **Frequency** – Number of transactions
- **Monetary** – Total spend
Then applied:
- Quantile-based segmentation to score customers into RFM buckets

---

## 🧠 Key Insights
- Major sales concentration in UK
- Sharp seasonal revenue patterns
- High-value customers can be profiled effectively using RFM metrics

---

