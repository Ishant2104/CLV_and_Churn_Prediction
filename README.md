# 🚀 Customer Churn & Lifetime Value Prediction  
## End-to-End Machine Learning & Business Decision Dashboard
![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)


<img width="436" height="293" alt="image" src="https://github.com/user-attachments/assets/c48e7f88-f723-481b-afa4-ec343de4d2ac" />

---
## Power BI Dashboard
<img width="851" height="481" alt="image" src="https://github.com/user-attachments/assets/b5e4f22b-902d-4ad1-a1e7-8e5534c1cda8" />


---

## 📌 Project Overview

This project builds an **end-to-end customer analytics system** that answers two critical business questions:

> **Which customers are likely to churn, and how much is each customer worth over the next 12 months?**

The solution combines:
- Customer Lifetime Value (CLV) modeling  
- Machine Learning–based churn prediction  
- An interactive **Power BI dashboard with What-If analysis**

The final outcome is a **decision-support system**, not just predictive models.

---

## 🎯 Business Objectives

- Predict customer churn probability  
- Estimate 12-month Customer Lifetime Value (CLV)  
- Segment customers by **risk and value**  
- Quantify **revenue at risk due to churn**  
- Simulate retention strategies using a **What-If discount model**

---

## 🧠 Key Concepts Used

- RFM Analysis (Recency, Frequency, Monetary)  
- Probabilistic CLV Modeling (BG/NBD + Gamma-Gamma)  
- Supervised Machine Learning for churn prediction  
- Business-oriented model evaluation  
- Decision analytics and simulation  

---

## 🗂️ Project Structure

```text
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── 01_Data_Preprocessing.ipynb
│   ├── 02_EDA.ipynb
│   ├── 03_Feature_Engineering.ipynb
│   ├── 04_CLV_Modeling.ipynb
│   ├── 05_Churn_Modeling.ipynb
│
├── powerbi/
│   └── Customer_Churn_CLV_Dashboard.pbix
│
├── assets/
│   └── dashboard.png
│
├── README.md
```

---

## 🔍 Phase-wise Breakdown

### Phase 1: Data Cleaning & Preparation
* Removed missing and invalid records
* Handled cancelled and returned transactions
* Created total_price = quantity × price
* Converted invoice dates to datetime format

### Phase 2: Exploratory Data Analysis (EDA)
* Customer purchase behavior analysis
* Revenue and order distribution analysis
* Outlier detection
* CLV skew and churn pattern analysis

### Phase 3: Feature Engineering
* RFM metrics per customer
* Purchase interval statistics
* Customer age features
* Log transformations for skewed variables
* One-time vs repeat buyer flags

### Phase 4: Customer Lifetime Value Modeling
* BG/NBD model to predict future purchase frequency
* Gamma-Gamma model to estimate average order value
* Generated 12-month CLV per customer

**📌 Why probabilistic models?**

*They are better suited for non-contractual retail data than standard regression approaches.*

### Phase 5: Churn Prediction
* Defined churn using inactivity-based logic
* Trained a supervised ML classifier (Random Forest / XGBoost)
* Features include RFM metrics, CLV, and behavioral signals
* Achieved ROC-AUC ≈ 0.95

📌 *Predictions are used for prioritization, not guarantees.*

### Phase 6: Power BI Dashboard & What-If Analysis
* Executive KPI cards
* Risk and revenue segmentation
* Risk vs Value scatter plot
* Interactive discount simulation
* Revenue saved vs discount cost analysis

---

## 📊 Power BI Dashboard Highlights
🔹 Key KPIs
* Total Customers
* Total CLV (12 Months)
* Revenue at Risk
* Average Churn Probability

🔹 Advanced Visualizations
* Customer Risk vs Lifetime Value Scatter Plot
* Customers by churn risk segment
* Revenue at risk by churn segment

🔹 What-If Discount Simulation
* Adjustable discount percentage slider
* Real-time impact on:
* Adjusted churn probability
* Revenue saved
* Discount cost
* Net business impact

📌 Key Insight:
Blanket discounts are often not cost-effective; targeted retention strategies provide better ROI.

---

## 🧠 Key Business Insights

* High churn risk does not always imply high revenue impact
* Many high-risk customers are low-value
* Medium-risk, high-CLV customers are the best retention targets
* Data-driven simulations prevent value-destructive decisions

---

### 🛠️ Tools & Technologies

* Python: Pandas, NumPy, Scikit-learn, Lifetimes
* SQL: Data extraction and aggregation
* Power BI: Interactive dashboard and simulations
* Jupyter Notebook: Analysis and modeling

--

## 📈 Model Performance

| Model | Metric |
|------|--------|
| Churn Prediction Model | ROC-AUC ≈ **0.95** |
| CLV Model | BG/NBD + Gamma-Gamma |

---

## 🧩 How to Run the Project

* Clone the repository
* Run notebooks in sequence (01 → 05)
* Export the final dataset
* Open the Power BI .pbix file

---

## 🚀 Future Improvements

* Targeted discount simulation by customer segment
* Time-varying churn modeling
* Uplift modeling for retention strategies
* Deployment via Streamlit or Power BI Service

---

## 👤 Author

Ishant Cane
Aspiring Data Scientist | Machine Learning & Analytics

⭐ Final Note

*This project focuses not only on predictive accuracy, but on business decision-making — transforming machine learning outputs into actionable insights.*

If you find this project useful, feel free to ⭐ the repository!
