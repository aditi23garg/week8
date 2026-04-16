# 🏥 Hospital Readmission Prediction — Week 08 (Tuesday)

## 📌 Overview

This assignment focuses on building a **30-day hospital readmission prediction system** using real-world messy healthcare data.

The workflow includes:

* Data quality audit and cleaning
* Feature engineering
* Building a **3-layer neural network from scratch using NumPy**
* Model evaluation using appropriate metrics
* Cost-based decision making for real-world hospital scenarios

---

## 🎯 Objective

To develop a robust pipeline that:

* Cleans and prepares hospital data
* Predicts whether a patient will be readmitted within 30 days
* Minimizes clinical risk using cost-sensitive decision making

---

## 📂 Dataset

* **hospital_records.csv**
* Contains patient demographics, clinical features, and hospital details
* Target column: `readmitted_30d`

---

## ⚙️ Technologies Used

* Python 3.x
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

---

## 📁 Folder Structure

```
week-08/
└── tuesday/
    ├── Assignment.ipynb
    ├── README.md
    └── .gitignore
```

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone <your-repo-link>
cd week-08/tuesday
```

---

### 2️⃣ Install Required Libraries

```bash
pip install numpy pandas scikit-learn matplotlib
```

---

### 3️⃣ Run the Notebook

```bash
jupyter notebook assignment.ipynb
```

---

### 4️⃣ Execution Order (IMPORTANT)

Run cells in the following sequence:

1. Data loading
2. Data audit
3. Data cleaning function + execution
4. Encoding & preprocessing
5. Neural network implementation
6. Training and evaluation
7. Cost-based threshold tuning

---

## 🧠 Key Implementation Details

### ✔ Data Cleaning

* Handled missing values using median imputation
* Converted data types to numeric
* Standardized categorical variables
* Removed outliers (BMI filtering)
* Extracted features from date column

---

### ✔ Neural Network (From Scratch)

* 3-layer architecture:

  * Input → Hidden (16) → Hidden (8) → Output
* Sigmoid activation function
* Binary Cross Entropy loss
* Forward + Backward propagation implemented manually

---

### ✔ Evaluation Strategy

* Accuracy avoided due to class imbalance
* Used:

  * Recall (priority)
  * F1-score
* Compared with Logistic Regression baseline

---

### ✔ Cost-Based Decision

* False Negative cost: ₹10,000
* False Positive cost: ₹1,000

Optimal threshold selected (~0.3) to:

* Minimize missed high-risk patients
* Reduce overall clinical cost

---

## 📊 Results

* Neural network successfully learned meaningful patterns
* Lower threshold improved recall significantly
* Model is suitable for real-world hospital decision-making

---

## ⚠️ Important Notes

* No hardcoded file paths used
* Modular functions implemented
* Proper preprocessing pipeline followed
* Code executes end-to-end without errors

---
