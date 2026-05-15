# Financial-Forecasting-Frontier-Distributed-ML

# 💻 Banking Data Analysis with Apache Spark – Data Parallelism Project

## 📌 Objective
The objective of this project is to demonstrate how **data parallelism in Apache Spark** can be used to process large-scale banking data efficiently. The dataset (`bank.csv`) contains client information related to marketing campaigns for term deposit subscriptions.

---

## 🗂️ Dataset Description

| Feature | Description |
|--------|------------|
| age | Age of the client |
| job | Type of job |
| marital | Marital status |
| education | Education level |
| default | Has credit in default? |
| balance | Account balance |
| housing | Has housing loan? |
| loan | Has personal loan? |
| contact | Type of communication |
| day | Last contact day |
| month | Last contact month |
| duration | Last contact duration |
| campaign | Number of contacts in current campaign |
| pdays | Days since last contact |
| previous | Number of previous contacts |
| poutcome | Outcome of previous campaign |
| y | Subscribed to term deposit (target) |

---

## ⚙️ Technologies Used
- Apache Spark  
- PySpark (Spark SQL, MLlib)  
- Google Colab  
- Python  

---

## 🚀 Project Workflow

### 1. 📊 Data Preparation and Partitioning
- Loaded dataset into Spark DataFrame  
- Used `repartition()` based on job column  

### 2. 🧠 Parallel Data Analysis
- Average balance per job using `groupBy()`  
- Top 5 age groups with most loans  

### 3. 🤖 Model Training
- Logistic Regression  
- `StringIndexer` for encoding  
- `VectorAssembler` for features  
- Train/test split  

### 4. 📈 Model Evaluation
- Accuracy  
- Precision  
- Recall  
- F1 Score  

### 5. 📡 Resource Monitoring
- Used `psutil` for CPU & memory tracking  

### 6. 📅 Task Scheduling
- Spark DAG scheduler  
- Lazy evaluation  

---

## ✅ Key Insights
- Age group **30–39** had the most loans  
- **Retired & students** had highest balances  
- Logistic Regression worked well with distributed data  

---

# 🤖 Machine Learning with Spark ML

## 🧠 Term Deposit Prediction

### 🎯 Objective
Build a **binary classification model** to predict term deposit subscriptions.

---

## 🔄 Workflow

### 1️⃣ Data Loading & EDA
- Loaded CSV into Spark DataFrame  
- Checked schema  

### 2️⃣ Preprocessing
- No missing values  
- Used `StringIndexer`  

### 3️⃣ Feature Engineering
- Used `VectorAssembler`  

### 4️⃣ Model Training
- Logistic Regression  
- 80/20 split  

### 5️⃣ Evaluation Metrics
- Accuracy: **89.17%**  
- Precision: **87.07%**  
- Recall: **89.17%**  
- F1 Score: **87.07%**  

### 6️⃣ Hyperparameter Tuning
- `ParamGridBuilder` + `CrossValidator`  
- Tuned Accuracy: **89.06%**

---

## 📊 Feature Importance

| Feature | Impact |
|--------|--------|
| poutcome | Strong Positive |
| housing | Moderate Positive |
| marital | Slight Positive |
| loan | Strong Negative |
| contact | Mild Negative |

---

## 📊 Key Insights
- Past campaign outcome is the strongest predictor  
- Housing loan increases subscription likelihood  
- Personal loan decreases subscription likelihood  

---

# 💳 Spark Data Processing Project – Bank Client Analysis

## 🎯 Objective
Analyze banking data using **Spark SQL and PySpark**

---

## 📌 Tasks

### ✅ Data Inspection
- Schema + summary stats  

### ✅ Data Transformation
- Filtered balance > 1000  
- Created quarter column  

### ✅ Aggregation
- Avg balance by job  
- Subscription count by marital status  

### ✅ UDF
- Age groups: `<30`, `30–60`, `>60`  

### ✅ Advanced Analysis
- Subscription rate by education  
- Loan default analysis  

### ✅ Visualization
- Bar charts & pie charts  

### ✅ Spark SQL
- Temp views + queries  

---

## 📊 Insights
- Older clients (>60) have highest balances  
- Most common job: Management  
- Best contact: Cellular  
- Default rate ~0.07%  

---

# 🔄 Real-Time Machine Learning with Spark Streaming

## 📌 Overview
Real-time simulation using **Spark Structured Streaming**

---

## ✅ Features

### 1️⃣ Stream Processing
- CSV chunk streaming  
- Real-time aggregations  

### 2️⃣ Real-Time Predictions
- Integrated ML model  

### 3️⃣ Window Operations
- 10-sec & 1-min windows  

### 4️⃣ Late Data Handling
- Watermarking  

---

## 🛠️ Tech Stack
- Spark Structured Streaming  
- PySpark  
- Pandas  
- Scikit-learn  
- Matplotlib  

---

# 💼 Banking Data Analysis (Pandas Version)

## 📌 Objective
Adapt Hadoop + Hive project using Pandas

---

## ✅ Tasks Covered
- Data inspection  
- Aggregations  
- Trends  
- Correlation  
- Anomaly detection  

---

## 📊 Key Insights
- Retired & management → high balances  
- May → most contacts  
- Previous success → higher conversions  
- Weak age-balance correlation  

---

## 📁 How to Run

```bash
pip install pyspark
```

### Steps
1. Open Google Colab / Jupyter  
2. Upload `bank.csv`  
3. Run all cells  

---

## 📦 Project Files
- README.md  
- Notebooks (.ipynb)  
- bank.csv  
- Screenshots  

---

## 📝 License
Educational use only  

---

## 🙋‍♂️ Author
**Nurandayya Bhavimath**  
📅 April 2026
