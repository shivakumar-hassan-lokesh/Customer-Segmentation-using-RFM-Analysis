# 🛒 Customer Segmentation using RFM Analysis  

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)  
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow?logo=pandas)  
![Scikit-Learn](https://img.shields.io/badge/ScikitLearn-Clustering-orange?logo=scikitlearn)  
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?logo=plotly)  
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal)  

---

## 📌 Project Overview  
This project focuses on **Customer Segmentation** using the **RFM (Recency, Frequency, Monetary) Analysis** method.  
The dataset is sourced from [Kaggle’s eCommerce dataset](https://www.kaggle.com/datasets/carrie1/ecommerce-data).  

RFM analysis is a proven marketing technique that helps businesses:  
- Identify **loyal customers**  
- Re-engage **at-risk customers**  
- Recognize **high-value buyers**  
- Tailor marketing strategies for **customer retention and growth**  

---

## 🎯 Objectives
- Clean and preprocess eCommerce transaction data  
- Calculate **RFM metrics** for each customer  
- Perform **quartile-based scoring** and **K-Means clustering**  
- Segment customers into actionable groups  
- Provide **business recommendations** based on insights  
- Visualize patterns and clusters  

---

## 📂 Dataset Details
- **Source:** [Kaggle – eCommerce Dataset](https://www.kaggle.com/datasets/carrie1/ecommerce-data)  
- **Size:** 541,909 rows × 8 columns  
- **Columns:**  
  - `InvoiceNo` → Invoice number  
  - `StockCode` → Product code  
  - `Description` → Product description  
  - `Quantity` → Number of items purchased  
  - `InvoiceDate` → Purchase date  
  - `UnitPrice` → Price per item  
  - `CustomerID` → Unique customer identifier  
  - `Country` → Customer’s country  

---

## ⚙️ Project Workflow
### 🔹 Step 1: Data Preprocessing  
- Handle missing values  
- Convert `InvoiceDate` to datetime  
- Remove cancelled/negative transactions  
- Create `TotalPrice = Quantity × UnitPrice`  

### 🔹 Step 2: RFM Calculation  
- **Recency (R):** Days since last purchase  
- **Frequency (F):** Number of unique transactions  
- **Monetary (M):** Total spend  

### 🔹 Step 3: RFM Scoring  
- Quartile-based scoring (1–4 scale)  
- Combined **RFM score**  
- Segments like **Champions, Loyal, At Risk, etc.**  

### 🔹 Step 4: K-Means Clustering  
- Standardized RFM values  
- Used **Elbow Method** to select optimal clusters  
- Created 4 clusters → High Value, New Customers, At Risk, Low Value  

### 🔹 Step 5: Profiling & Recommendations  
- **High Value Loyal** → Reward with VIP offers, personalization  
- **New Customers** → Welcome campaigns, first-purchase discounts  
- **At Risk** → Re-engagement campaigns, win-back offers  
- **Low Value** → Cost-efficient promotions, upselling  

---

## 📊 Visualizations
### RFM Distributions  
![Boxplots](assets/rfm_boxplot.png)  

### KMeans Segmentation  
![Scatter Plot](assets/kmeans_scatter.png)  

### Heatmap of Monetary Value  
![Heatmap](assets/rfm_heatmap.png)  

### Customer Segment Distribution  
![Pie Chart](assets/segment_pie.png)  

---

## 📈 Key Insights
- **Champions** represent ~15% of customers but generate ~50% of revenue  
- **At Risk** customers show high past value but reduced activity → targeted win-back is essential  
- **New Customers** need nurturing campaigns for retention  
- **Low Value** group contributes minimally but can be nudged with bundles & discounts  

---

## 🛠️ Tech Stack
- **Python 3.9+**  
- **Pandas, NumPy** → Data wrangling  
- **Matplotlib, Seaborn** → Visualization  
- **Scikit-Learn** → KMeans clustering  
- **Jupyter Notebook** → Development & analysis  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/Customer-Segmentation-RFM.git
   cd Customer-Segmentation-RFM
