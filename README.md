# 🧠 Causal Demand Shock Attribution System

An advanced, explainable data science system that not only **detects demand anomalies**, but also **attributes their root causes**—such as trend shifts, seasonality noise, or external shocks—using time-series analysis and machine learning.

---

## 📌 Project Motivation

Traditional demand anomaly detection systems answer **what happened**, but fail to explain **why it happened**.

In real-world supply chain and demand forecasting scenarios, decision-makers need:
- Clear explanations behind demand spikes or drops  
- Separation of natural seasonality from real external shocks  
- Quantified severity of demand disruptions  

This project addresses that gap by building a **causal attribution layer on top of anomaly detection**.

---

## 🎯 Key Objectives

- Detect abnormal demand behavior in time-series data  
- Engineer causal features that explain demand fluctuations  
- Attribute each anomaly to a meaningful root cause  
- Quantify the severity of demand shocks  
- Generate explainable, business-ready insights  

---

## 🏗️ Project Architecture

Causal-Demand-Shock-Attribution/
│
├── data/
│ ├── raw_demand.csv
│ ├── large_demand_data.csv
│ ├── events_data.csv
│ └── causal_features.csv
│
├── notebooks/
│ ├── anomaly_detection.ipynb
│ ├── baseline_demand_model.ipynb
│ ├── data_preparation.ipynb
│ ├── causal_feature_engineering.ipynb
│ ├── shock_attribution_model.ipynb
│ └── explanation_and_insights.ipynb
│
└── README.md


---

## 🧪 Methodology Overview

### 1️⃣ Demand Anomaly Detection
- Used statistical signals and Isolation Forest  
- Identified abnormal demand points in time-series data  

### 2️⃣ Baseline Demand Modeling
- Decomposed demand into:
  - Trend  
  - Seasonality  
  - Residual components  

### 3️⃣ Causal Feature Engineering
Engineered interpretable features such as:
- Lag-based demand features  
- Rolling statistics (mean & standard deviation)  
- Z-score deviations  
- Trend change magnitude  
- Residual intensity  

### 4️⃣ Shock Attribution Logic
Each anomaly is attributed to one of:
- **Trend Shift** – long-term structural change  
- **Seasonality Noise** – expected cyclical variation  
- **External Shock** – sudden, abnormal disruptions  

### 5️⃣ Shock Severity Scoring
Computed a weighted severity score using:
- Statistical deviation (z-score)  
- Residual strength  
- Trend change impact  

### 6️⃣ Explainability & Insights
- Aggregated severity by shock type  
- Identified dominant causes of demand instability  
- Produced decision-ready insights  

---

## 📊 Example Insights Generated

- External shocks caused the **highest average demand disruption**  
- Trend shifts resulted in **long-term demand realignment**  
- Seasonal noise produced frequent but low-severity fluctuations  

These insights help organizations:
- React faster to true demand shocks  
- Avoid overreacting to seasonal patterns  
- Improve inventory and supply chain planning  

---

## 🛠️ Tech Stack

- **Programming:** Python  
- **Data Analysis:** Pandas, NumPy  
- **Visualization:** Matplotlib  
- **ML Models:** Isolation Forest  
- **Time-Series Analysis:** Rolling statistics, decomposition  
- **Environment:** Jupyter Notebook  

---

## ▶ How to Run

Run the notebooks in the following order to reproduce the full pipeline:

1. anomaly_detection.ipynb  
2. baseline_demand_model.ipynb  
3. data_preparation.ipynb  
4. causal_feature_engineering.ipynb  
5. shock_attribution_model.ipynb  
6. explanation_and_insights.ipynb  

---

## 📈 Why This Project Stands Out

- Goes beyond anomaly detection by explaining *why* demand shocks occur  
- Focuses on causality and interpretability, not just predictions  
- Reflects real-world supply chain and business analytics problems  
- Designed for decision-makers, not just model accuracy  

---

## 📌 Future Enhancements

Integrate external event data (holidays, promotions, disruptions)

Apply causal inference frameworks (DoWhy, CausalImpact)

Build a dashboard for real-time monitoring

Extend to multivariate demand scenarios

---

## 🚀 How to Run the Project

```bash
git clone https://github.com/your-username/Causal-Demand-Shock-Attribution-System.git
cd Causal-Demand-Shock-Attribution-System