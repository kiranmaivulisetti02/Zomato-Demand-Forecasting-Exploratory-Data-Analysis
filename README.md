 Zomato Demand Forecasting & Exploratory Data Analysis

 Recruiter Snapshot (FAANG / Service Companies)

**Domain:** Data Analytics | Machine Learning | Time Series Forecasting
**Core Skills:** Python, Pandas, SQL-ready data prep, EDA, SARIMA, LSTM, Model Evaluation
**Business Use Case:** Demand forecasting for operational and strategic decision-making

**What this project demonstrates (quick scan):**

* End-to-end analytics workflow (raw data → insights → forecasting)
* Statistical + Deep Learning model comparison
* Strong business framing of technical results
* Production-aligned evaluation using MAE & RMSE

---

 Project Overview

This project demonstrates an **end-to-end data analytics and machine learning workflow** using Zomato restaurant data. The objective is to analyze restaurant popularity patterns and forecast demand using both **statistical** and **deep learning** time-series models.

Due to the absence of an explicit timestamp column, **restaurant votes are treated as a proxy for demand**, and the dataset index is used as a sequential time dimension. This assumption is clearly stated and justified, aligning with standard academic and portfolio practices.

---

 Objectives

* Perform **Exploratory Data Analysis (EDA)** to understand demand patterns
* Preprocess and clean real-world business data
* Build and compare **SARIMA** and **LSTM** forecasting models
* Evaluate models using **MAE** and **RMSE** metrics
* Translate analytical results into **business insights**

---

 Dataset Description

**Source:** Zomato restaurant dataset

**Key Columns Used:**

* `name` – Restaurant name
* `votes` – Number of user votes (used as demand proxy)
* `rate` – Restaurant rating
* `approx_cost(for two people)` – Cost indicator
* `online_order` – Online ordering availability
* `book_table` – Table booking availability
* `listed_in(type)` – Restaurant category

---

 Tools & Technologies

* **Programming:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Time Series Modeling:** Statsmodels (SARIMA)
* **Deep Learning:** TensorFlow / Keras (LSTM)
* **Evaluation Metrics:** MAE, RMSE
* **Reporting:** Jupyter Notebook, PDF report

---

 Exploratory Data Analysis (EDA)

* Demand distribution analysis using histograms
* Trend visualization of restaurant popularity
* Correlation analysis between votes, ratings, and cost
* Handling missing values and feature standardization

EDA helped identify demand variability and informed model selection.

---

 Forecasting Models

 1. SARIMA (Statistical Model)

* Captures trend and seasonality
* Suitable for structured and linear time-series data
* Interpretable and effective for short-term forecasting

 2. LSTM (Deep Learning Model)

* Recurrent Neural Network capable of learning nonlinear patterns
* Uses sequence modeling and scaled inputs
* Suitable for complex and dynamic demand behavior

---

  Model Evaluation

Both models were evaluated using an **80/20 train-test split**.

**Evaluation Metrics:**

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**

A comparative analysis highlights the strengths and limitations of each approach in a business context.

---

Key Business Insights

* SARIMA performs well for stable, short-term demand forecasting
* LSTM captures nonlinear demand patterns more effectively
* Demand forecasting can support:

  * Inventory and workforce planning
  * Restaurant performance analysis
  * Data-driven operational decisions

---

## Repository Structure

```
├── README.md
├── Zomato_EDA_LSTM_Forecasting.ipynb
└── data/
    └── Zomato-data.csv
```

---

##  How to Run

1. Clone the repository
2. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels scikit-learn tensorflow
   ```
3. Open the notebook:

   ```bash
   jupyter notebook Zomato_EDA_LSTM_Forecasting.ipynb
   ```

---

## Author

**Kiranmai Vulisetti**
Aspiring Data Analyst / ML Associate

---

##  Future Enhancements

* Incorporate real timestamped order data
* Add external factors (location, cuisine, promotions)
* Deploy model using Flask or FastAPI
* Automate forecasting pipeline

---

⭐ If you find this project useful, feel free to star the repository!
