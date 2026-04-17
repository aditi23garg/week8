# 📊 Social Media Moderation System — Week 08 (Wednesday)

## 📌 Overview

This assignment focuses on building a **content moderation system** using:

* **CNN (Convolutional Neural Networks)** for image classification (MNIST)
* **Text classification + semantic search** for social media moderation

The system is designed to:

* Detect harmful or negative content
* Retrieve semantically similar posts even without keyword overlap

---

## 🎯 Objective

To develop a **two-stage moderation pipeline** that:

1. Classifies sentiment of social media posts
2. Uses semantic similarity to identify related harmful content
3. Improves detection of posts that evade keyword-based filters

---

## 📂 Dataset

### 1. Social Media Dataset

* **Twitter_Data.csv**
* Columns:

  * `clean_text` → text data
  * `category` → sentiment label:

    * `1` → Positive
    * `0` → Neutral
    * `-1` → Negative

---

### 2. MNIST Dataset

* Handwritten digit dataset (0–9)
* Used for CNN implementation

---

## ⚙️ Technologies Used

* Python 3.x
* NumPy
* Pandas
* Scikit-learn
* TensorFlow / Keras
* SentenceTransformers
* Matplotlib

---

## 📁 Folder Structure

```id="jzgrso"
week-08/
└── wednesday/
    ├── Twitter_Data.csv
    ├── Assignment.ipynb
    ├── README.md
```

---

## 🚀 How to Run the Project

### 1️⃣ Clone Repository

```bash id="tr5qsy"
git clone <https://github.com/aditi23garg/week8/new/main/wednesday>
cd week-08/wednesday
```

---

### 2️⃣ Install Dependencies

```bash id="a19s41"
pip install numpy pandas scikit-learn matplotlib tensorflow sentence-transformers
```

---

### 3️⃣ Run Notebook

```bash id="ld8p6v"
jupyter notebook assignment.ipynb
```

---

### 4️⃣ Execution Order (IMPORTANT)

Run cells sequentially:

1. Load and audit social media dataset
2. Clean and preprocess text data
3. Load and preprocess MNIST dataset
4. Train CNN model
5. Build sentiment classifier (TF-IDF + Logistic Regression)
6. Build semantic similarity system (embeddings)
7. Combine into two-stage moderation pipeline
8. Evaluate results

---

## 🧠 Key Implementation Details

### ✔ Data Cleaning

* Removed missing labels (`category`)
* Handled missing text values
* Ensured correct label encoding (-1, 0, 1)

---

### ✔ Sentiment Classification

* TF-IDF vectorization used for text representation
* Logistic Regression used for multi-class classification
* `class_weight='balanced'` used to handle class imbalance

---

### ✔ CNN Model (MNIST)

* 2 convolutional layers for feature extraction
* MaxPooling layers for dimensionality reduction
* Dense layers for classification

---

### ✔ Semantic Similarity System

* Sentence embeddings using `SentenceTransformer`
* Cosine similarity used to find similar posts
* Captures semantic meaning beyond keywords

---

### ✔ Two-Stage Moderation Pipeline

* **Stage 1:** Sentiment classifier identifies negative/harmful posts
* **Stage 2:** Semantic search retrieves similar posts

👉 Improves recall and detects hidden harmful content

---

## 📊 Evaluation Strategy

* Accuracy is avoided due to class imbalance
* Metrics used:

  * Precision
  * Recall
  * F1-score

👉 Recall is prioritized to ensure harmful posts are not missed

---

## 📈 Results

* Classifier successfully detects sentiment patterns
* Semantic search retrieves contextually similar posts
* Combined system improves detection performance

**Aditi Garg**
PG Diploma — AI/ML & Agentic AI Engineering
IIT Gandhinagar

---
