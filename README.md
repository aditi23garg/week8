# 📊 Week 08 — Monday Assignment

**Time Series Analysis & Sensor Failure Prediction**

---

## 🧾 Overview

This assignment focuses on **time series analysis and modeling** using real-world datasets. It covers:

* Understanding time series properties (trend, seasonality, stationarity)
* Data cleaning and preprocessing for sequential data
* Building forecasting models (ARIMA, SARIMA)
* Predicting equipment failure using sensor data
* Translating model outputs into actionable business insights

---

## 📂 Datasets Used

1. **E-commerce Orders Dataset**

   * Used to generate daily sales time series
   * Based on order timestamps

2. **Sensor Dataset**

   * Contains multiple sensor readings over time
   * Used to predict equipment failure

> Note: Datasets are provided via LMS and should be placed in the project directory before running the notebook.

---

## 🧠 Tasks Performed

### 🟢 Easy

* Time series characterization (trend, seasonality, stationarity)
* Data cleaning and preprocessing of sensor data

### 🟡 Medium

* ARIMA model for baseline forecasting
* SARIMA model for seasonal patterns
* Sensor failure prediction using classification model

---

## ⚙️ Technologies Used

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Statsmodels
* Scikit-learn

---

## 📁 Folder Structure

```
week-08/
└── monday/
    ├── Assignment.ipynb
    ├── README.md
    └── .gitignore
```

---

## 🚀 How to Run

### 1️⃣ Clone Repository

```bash
git clone <your-repo-link>
cd week-08/monday
```

---

### 2️⃣ Install Dependencies

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn
```

---

### 3️⃣ Add Dataset

* Place the following files inside the folder:

  * `sensor.csv`
  * `olist_orders_dataset.csv`

---

### 4️⃣ Run Notebook

```bash
jupyter notebook
```

Open:

```
assignment.ipynb
```

Run all cells sequentially.

---

## 📊 Key Highlights

* Time series data requires **temporal order preservation** (no random split)
* ARIMA captures trend, while SARIMA captures **seasonality**
* Sensor failure prediction prioritizes **Recall** due to high cost of missed failures
* Data cleaning is critical to avoid empty datasets and model errors

---


## ✅ Conclusion

This assignment demonstrates:

* End-to-end time series workflow
* Model selection based on data characteristics
* Practical application of ML for real-world problems


