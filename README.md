# GST Fraud Detection in Billing

A machine learning-based system designed to identify suspicious GST billing transactions and detect potentially fraudulent patterns in transaction data.

## 📌 Overview

GST billing involves a large volume of transactions, making it challenging to manually identify unusual or suspicious billing activity.

This project explores how machine learning can assist in this process by analyzing transaction data, learning patterns from historical records, and identifying transactions that may require further investigation.

The system uses **Random Forest and XGBoost** classification models to analyze billing patterns and distinguish between genuine and potentially fraudulent transactions.

> The system is intended as a fraud-screening and analysis tool. A model prediction alone does not establish that a transaction is fraudulent.

## 🎯 Objectives

- Detect suspicious GST billing transactions.
- Identify abnormal patterns in transaction data.
- Prepare and preprocess billing datasets for machine learning.
- Train and compare classification models.
- Evaluate model performance using relevant classification metrics.
- Provide a foundation for automated GST fraud screening.

## 🧠 Machine Learning Approach

The project follows a machine learning pipeline that transforms raw billing data into useful predictions:

```text
Billing Transaction Data
          │
          ▼
   Data Preprocessing
          │
          ▼
    Feature Preparation
          │
          ▼
     Train / Test Split
          │
          ▼
 ┌──────────────────────┐
 │   Machine Learning   │
 │       Models         │
 │                      │
 │  Random Forest       │
 │  XGBoost             │
 └──────────┬───────────┘
            │
            ▼
     Model Evaluation
            │
            ▼
   Fraud / Suspicion
       Prediction
```

### Random Forest

Random Forest is used as a tree-based ensemble classification approach. It combines multiple decision trees to make predictions and provides a useful model for comparison with other machine learning techniques.

### XGBoost

XGBoost is another tree-based ensemble model used for classification. It is particularly effective for structured and tabular datasets and can capture complex relationships between transaction features.

Using both models allows the project to experiment with different approaches and compare their performance on the available billing data.

## 📊 Model Evaluation

The models can be evaluated using classification metrics such as:

- **Accuracy** — Overall proportion of correct predictions.
- **Precision** — Proportion of predicted suspicious transactions that are actually suspicious.
- **Recall** — Proportion of suspicious transactions successfully identified.
- **F1-Score** — Balance between precision and recall.
- **Confusion Matrix** — Detailed view of correct and incorrect predictions.

For fraud detection, precision and recall are particularly important because both false positives and missed suspicious transactions can have practical consequences.

## 🛠️ Tech Stack

### Programming
- Python

### Machine Learning
- Scikit-learn
- Random Forest
- XGBoost

### Data Processing
- Pandas
- NumPy

### Backend
- Flask

### Database
- SQLite

### Development Tools
- Jupyter Notebook
- VS Code
- Git & GitHub

## ✨ Key Features

- 🔍 Suspicious GST transaction detection
- 🤖 Machine learning-based fraud classification
- 🌲 Random Forest model
- ⚡ XGBoost model
- 📊 Model performance evaluation
- 🧹 Transaction data preprocessing
- 🗃️ SQLite database integration
- 🌐 Flask-based application interface

## 📂 Project Structure

```text
GST-Fraud-detection-in-billing/
│
├── data/
│   └── Dataset files
│
├── models/
│   └── Trained ML models
│
├── notebooks/
│   └── Data analysis and model development
│
├── static/
│   └── CSS / frontend assets
│
├── templates/
│   └── HTML templates
│
├── app.py
├── requirements.txt
├── README.md
└── ...
```

> Update the structure above if your repository uses different folder or file names.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Manohar-L-U/GST-Fraud-detection-in-billing.git
```

### 2. Navigate to the project

```bash
cd GST-Fraud-detection-in-billing
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

**Windows:**

```bash
venv\Scripts\activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

## ▶️ Running the Application

Start the Flask application:

```bash
python app.py
```

Then open the local application URL displayed in the terminal.

## 🔄 Project Workflow

```text
        ┌─────────────────┐
        │ Billing Dataset │
        └────────┬────────┘
                 │
                 ▼
       ┌──────────────────┐
       │ Data Preprocessing│
       └────────┬─────────┘
                │
                ▼
       ┌──────────────────┐
       │ Feature Engineering│
       └────────┬─────────┘
                │
                ▼
       ┌──────────────────┐
       │ Model Training   │
       └────────┬─────────┘
                │
        ┌───────┴────────┐
        ▼                ▼
 ┌─────────────┐  ┌─────────────┐
 │Random Forest│  │   XGBoost   │
 └──────┬──────┘  └──────┬──────┘
        │                │
        └───────┬────────┘
                ▼
       ┌──────────────────┐
       │ Model Evaluation │
       └────────┬─────────┘
                │
                ▼
       ┌──────────────────┐
       │ Fraud Screening  │
       └──────────────────┘
```

## 🔮 Future Improvements

- Integrate larger and more diverse GST transaction datasets.
- Compare additional fraud detection algorithms.
- Add real-time transaction monitoring.
- Improve feature engineering for complex billing patterns.
- Develop an interactive fraud analytics dashboard.
- Add explainable AI to understand individual predictions.
- Implement automated model retraining with new transaction data.
- Deploy the application to a cloud platform.

## 👨‍💻 Author

**Manohar L U**

Computer Science & Design Engineer  
Java Full Stack & AI Developer

- GitHub: [Manohar-L-U](https://github.com/Manohar-L-U)
- LinkedIn: [Manohar L U](https://www.linkedin.com/in/manohar-l-u-727b88268)
- LeetCode: [ManoharLU731](https://leetcode.com/ManoharLU731)

## 📄 License

This project is developed for educational and portfolio purposes.
