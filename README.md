# 📊 Trader Behavior vs Market Sentiment Analysis

## 🧠 About This Project

This repository contains my **Data Science internship project notebook**, where I analyze how **market sentiment (Fear vs Greed)** affects **trader behavior** in the cryptocurrency market.

The analysis is fully implemented in **`notebook_1.ipynb`** using Python and Google Colab, following a structured, step-by-step workflow.

---

## 🎯 Problem Statement

Market sentiment strongly influences trading decisions.
This project aims to understand:

* How trader profitability changes during Fear vs Greed phases
* Whether traders take higher risk (leverage, size) during Greed
* How trading volume and behavior vary with sentiment

The goal is to identify **behavioral patterns** that can support smarter trading strategies.

---

## 📁 Repository Structure

```
ds_mohd_osama/
├── notebook_1.ipynb        # Complete analysis notebook (main file)
├── csv_files/              # Cleaned & merged datasets generated in notebook
│   └── merged_data.csv
├── outputs/                # Charts and visualizations saved from notebook
│   └── *.png
├── ds_report.pdf           # Final summarized insights
└── README.md               # Project overview (this file)
```

---

## 📊 Datasets Used

### 1️⃣ Market Sentiment Dataset

* Contains daily Bitcoin sentiment data
* Classified as **Fear** or **Greed**
* Used to represent overall market psychology

### 2️⃣ Historical Trader Dataset

* Trade-level execution data
* Includes:

  * Execution price
  * Trade size
  * Leverage
  * Closed PnL
  * Timestamps
* Used to study real trader behavior

---

## 🛠️ Notebook Workflow (As Implemented)

The notebook follows this exact sequence:

1️⃣ **Data Loading**

* Loaded sentiment and trader datasets
* Initial inspection using `.head()`, `.info()`, `.describe()`

2️⃣ **Data Cleaning & Preprocessing**

* Timestamp conversion and alignment
* Removal of invalid or missing trade records
* Standardization of sentiment labels

3️⃣ **Feature Engineering**

* Trade volume calculation
* Profit/loss indicators
* Risk representation using leverage

4️⃣ **Data Merging**

* Sentiment data merged with trader data using date alignment
* Each trade mapped to corresponding market sentiment

5️⃣ **Exploratory Data Analysis (EDA)**

* Profitability comparison across Fear vs Greed
* Leverage and risk behavior analysis
* Volume and distribution analysis using visualizations

6️⃣ **Insights & Interpretation**

* Behavioral differences identified
* Risk-reward patterns analyzed

---

## 📈 Key Observations

* Traders generally use **higher leverage during Greed phases**
* Increased trading activity does **not always improve profitability**
* Fear phases show **more controlled and stable outcomes**
* High leverage often amplifies losses rather than gains

---

## 🏁 Conclusion

The notebook demonstrates that **market sentiment significantly impacts trader behavior**.
While Greed encourages aggressive trading, disciplined strategies during Fear phases may lead to better risk-adjusted performance.

This analysis highlights the importance of **emotion-aware trading strategies** in crypto markets.

---

## 🚀 Future Improvements

* Include Extreme Fear & Extreme Greed categories
* Perform trader-level clustering
* Build predictive models using sentiment features
* Backtest sentiment-based trading strategies

---

## 🧰 Tools & Environment

* Python
* Pandas, NumPy
* Matplotlib / Seaborn
* Google Colab

---

## 📌 Notes

* All analysis is contained in `notebook_1.ipynb`
* Charts generated in the notebook are saved in the `outputs/` folder
* Notebook access is set to **public (view-only)** as required

## Google Colab Notebook
https://colab.research.google.com/drive/1qCfNs4VPt1Z0nyfmE6RefY2ykUtFuQ-W?usp=sharing
