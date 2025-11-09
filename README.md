### 🧠 Customer Segmentation & Sales Forecasting – Online Retail

---


## 📋 Project Overview

This project performs data-driven analysis of online retail transactions to uncover customer purchasing behavior and forecast future sales trends.
The analysis is divided into two major components:
- Customer Segmentation using RFM analysis and K-Means clustering.

- Sales Forecasting using SARIMAX and Prophet time series models.

---


## 🧾 Dataset

**Source:** Online Retail II Dataset (Kaggle)

**Description:**
This dataset contains transactional data from a UK-based online retailer. It includes fields such as:

**InvoiceNo –** Transaction identifier

**StockCode –** Product code

**Description –** Product description

**Quantity –** Units purchased

**InvoiceDate –** Date of purchase

**UnitPrice –** Price per unit

**CustomerID –** Unique ID for each customer

**Country –** Country of customer

---


## ⚙️ Technologies Used

Python 3.x

## Libraries:

**pandas, numpy –** Data cleaning and manipulation

**matplotlib, seaborn –** Visualization

**sklearn –** Clustering and preprocessing

**Prophet, statsmodels –** Time series forecasting

**math –** RMSE and MAPE calculations

---


## 🧹 Data Preprocessing

**Loaded the cleaned dataset:** online_retail_II cleaned.csv

- Handled missing values and data type conversions.

- Converted InvoiceDate to datetime format.

- Created additional features: Year, Month, and Day.

- Calculated TotalAmount = Quantity * UnitPrice.

- Filtered out negative or cancelled transactions.

---


## 📊 Exploratory Data Analysis (EDA)

**Monthly Revenue Analysis:** Visualized monthly sales trends.

**Top Products:** Identified top 10 best-selling products by total revenue.

**Country-wise Sales:** Compared customer contribution by country.

**Customer Activity:** Assessed purchasing frequency and average order values.

---


## 👥 Customer Segmentation (RFM + K-Means)

## RFM Metrics:

**Recency:** Days since last purchase

**Frequency:** Number of purchases

**Monetary:** Total amount spent

**Approach:**

- Normalized features using StandardScaler.

- Applied K-Means Clustering to segment customers into groups.

- Used PCA for dimensionality reduction and cluster visualization.

**Outcome:**

- Customers grouped into meaningful segments (e.g., high-value loyal customers vs. infrequent buyers).

---


## 📈 Sales Forecasting

**Models Used:**

- SARIMAX (Seasonal ARIMA with Exogenous Variables)

- Prophet (by Meta)

**Process:**

- Aggregated daily and monthly sales totals.

- Trained models to capture seasonality and trend.

- Evaluated model accuracy using RMSE and MAPE.

**Results:**

- Generated short-term and long-term forecasts for sales prediction.

- Identified sales peaks during seasonal periods.

## 📑 Key Insights

- Monthly revenue fluctuates seasonally, peaking around holidays.

- A small group of customers contributes to a large proportion of revenue (Pareto principle).

- SARIMAX provided slightly better short-term accuracy, while Prophet handled long-term seasonality well.

---


## 📁 Project Structure
Online_retail_Analysis.ipynb        # Main analysis notebook
online_retail_II cleaned.csv # Cleaned dataset
README.md                   # Project documentation

---


## 📜 License
This project is licensed under the [MIT License](LICENSE).  

---

## 📧 Contact
👤 **Vedika Sankhe**  
🔗 [GitHub](https://github.com/VedikaaSankhe) | [LinkedIn](https://www.linkedin.com/in/vedika-sankhe-707700317)  

⭐ *If you found this project useful, don’t forget to star the repo!*  
