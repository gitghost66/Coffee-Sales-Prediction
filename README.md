# ☕ **Coffee Sales Forecasting**

> *Brew insights from your data and serve predictions fresh!*

---

## 📖 **Overview**

The **Coffee Sales Forecasting** project is all about transforming historical coffee shop sales data into actionable insights and accurate predictions.
By analyzing transaction patterns and building predictive models, this project aims to help businesses:

* Understand **sales trends** over time
* Identify **best-selling products** and **peak hours**
* Forecast **future sales** for better inventory and staffing decisions

This repository includes:

✅ **Data Cleaning & Preprocessing**
✅ **Exploratory Data Analysis (EDA)**
✅ **Interactive Visualizations**
✅ **Predictive Machine Learning Models**

---

## 📂 **Project Structure**

```
Coffee-Sales-Forecasting/
│
├── notebooks/
│   ├── coffee_analysis.ipynb      # EDA & forecasting workflow
│   └── data/
│       └── coffee_sales.csv        # Raw transaction dataset
│
├── plots/                         # Generated charts & visualizations
├── env/                           # Python virtual environment
├── README.md                      # This file
└── .git/                          # Git metadata
```

---

## 📊 **Dataset Description**

**Source:** `notebooks/data/coffee_sales.csv`

| Column        | Description                      |
| ------------- | -------------------------------- |
| `date`        | Transaction date (`YYYY-MM-DD`)  |
| `datetime`    | Exact purchase timestamp         |
| `cash_type`   | Payment method (`cash` / `card`) |
| `card`        | Anonymized customer ID           |
| `money`       | Transaction amount               |
| `coffee_name` | Coffee type purchased            |

---

## 🔍 **Exploratory Data Analysis Highlights**

The EDA uncovers key insights into coffee sales patterns:

* **📈 Sales Trends Over Time** → Daily, weekly, and monthly revenue tracking
* **☕ Coffee Type Popularity** → Which drinks keep customers coming back
* **💳 Payment Preferences** → Cash vs. card usage
* **⏰ Peak Purchase Hours** → Optimal staffing and promotions window
* **👥 Customer Retention** → Identifying repeat buyers and spend patterns

### Example Visuals:

* **Line Charts** → Revenue trends over time
* **Bar Charts** → Best-selling coffee types
* **Heatmaps** → Hourly sales distribution

---

## 🤖 **Machine Learning Forecasting**

### **Workflow**

1. **Feature Engineering**

   * Extract `day`, `month`, `hour`, `weekday` from `datetime`
   * Encode categorical features (`coffee_name`, `cash_type`)

2. **Models Used**

   * **Baseline:** Linear Regression
   * **Advanced:** Random Forest, XGBoost

3. **Evaluation Metrics**

   * **MAE** (Mean Absolute Error)
   * **RMSE** (Root Mean Squared Error)
   * **R² Score** (Explained Variance)

---

## ⚙️ **Setup & Installation**

```bash
# 1️⃣ Clone the repo
git clone <repo-url>
cd Coffee-Sales-Forecasting

# 2️⃣ Create & activate a virtual environment
python -m venv env
source env/bin/activate     # Mac/Linux
env\Scripts\activate        # Windows

# 3️⃣ Install dependencies
pip install -r requirements.txt

# 4️⃣ Launch Jupyter Notebook
jupyter notebook
```

---

## 🚀 **Usage Guide**

1. Open `notebooks/coffee_analysis.ipynb`
2. Run the cells to:

   * Explore data
   * Visualize trends
   * Train predictive models
3. Update `coffee_sales.csv` to forecast new sales data
4. Check the `plots/` folder for generated visuals

---

## 📈 **Key Results**

* **Top-selling coffees:** Latte, Americano, Hot Chocolate
* **Peak hours:** **10 AM – 2 PM** drive most sales
* **Model performance:** \~**90% R² score** on test data

---

## 🚀 **Future Enhancements**

* 📡 **Real-time Forecasting** – Stream sales data live for instant predictions
* 🌦 **Seasonality Analysis** – Detect holiday or seasonal demand spikes
* 🌐 **Interactive Dashboard** – Deploy via Streamlit or Flask
* 🎯 **Customer Segmentation** – Personalize promotions for different buyer groups

---

