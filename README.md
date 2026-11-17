# Customer Churn Analysis
**B.Tech Project | Computer Science & Engineering**
**The ICFAI University, Jaipur | 2025-2026**

| | |
|---|---|
| **Authors** | Dhruv Gupta & Anurag Sagar |
| **Guide** | Prof. Mr. Abizer Safdari |
| **Department** | Faculty of Science and Technology, IcfaiTech |

---

## 📌 Project Overview

This project analyzes customer churn in subscription-based businesses using Python.
It identifies key behavioral drivers of churn (tenure, pricing, support friction)
and provides a predictive machine learning model to flag at-risk customers.

---

## 🗂️ Project Structure

```
customer_churn_project/
├── app.py              ← Streamlit interactive dashboard (main deliverable)
├── analysis.py         ← Standalone terminal analysis script
├── requirements.txt    ← Python dependencies
├── README.md           ← This file
└── charts/             ← Auto-generated charts (created on first run)
```

---

## 🚀 How to Run

### Option A — Interactive Dashboard (Recommended)

```bash
# Step 1: Install dependencies
pip install -r requirements.txt

# Step 2: Launch the dashboard
streamlit run app.py
```
The browser will open automatically at `http://localhost:8501`

### Option B — Terminal Analysis Script

```bash
python analysis.py
```
This will:
- Generate the dataset (or load `customer_churn.csv` if present)
- Perform EDA and save 8 charts to the `charts/` folder
- Train a Logistic Regression model and print metrics

---

## 🔬 Methodology

| Phase | Description |
|---|---|
| **1. Data Collection** | Synthetic dataset generated from realistic churn probability formulas |
| **2. Preprocessing** | Null removal, label encoding, feature engineering |
| **3. EDA** | Churn distribution, tenure, charges, support ticket analysis, correlation heatmap |
| **4. ML Model** | Logistic Regression with train/test split (80/20), ROC-AUC evaluation |
| **5. Dashboard** | Interactive Streamlit app with live churn predictor |

---

## 📊 Key Findings

- **Churn Rate:** ~36% of customers churn (above 26% industry average)
- **Tenure:** Churned customers have ~7 months lower average tenure — first 0–3 months is the "danger zone"
- **Monthly Charges:** Higher charges correlate with churn — price sensitivity is significant
- **Support Tickets:** Churned customers file more support tickets — unresolved frustration drives exits

---

## 🛠️ Technologies Used

| Library | Purpose |
|---|---|
| **Pandas** | Data manipulation and cleaning |
| **NumPy** | Numerical operations |
| **Matplotlib** | Base plotting engine |
| **Seaborn** | Statistical visualizations |
| **Scikit-learn** | Logistic Regression, evaluation metrics |
| **Streamlit** | Interactive web dashboard |

---

## 📚 References

1. McKinney, W. (2010). *Data Structures for Statistical Computing in Python.*
2. Waskom, M. L. (2021). *Seaborn: statistical data visualization.*
3. Hunter, J. D. (2007). *Matplotlib: A 2D graphics environment.*
4. Official Python Documentation: https://docs.python.org/3/
5. Pandas Documentation: https://pandas.pydata.org/

---

*Submitted in fulfillment of the B.Tech (CSE) requirements at The ICFAI University, Jaipur.*
