# Credit Scoring Model (Credit Risk AI)

[![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![CodeAlpha](https://img.shields.io/badge/Internship-CodeAlpha-blueviolet)](https://github.com/PRANS009)

A machine learning project developed for the **CodeAlpha Data Science Internship**, focused on credit risk assessment and credit scoring. The project analyzes customer financial behaviors, payment history, and demographic profiles to predict the likelihood of credit card default.

---

## 📌 Project Overview

Credit scoring models are fundamental tools utilized by banks and financial institutions to evaluate the risk associated with lending money. This project provides:
- **Exploratory Data Analysis (EDA)**: Understanding data distributions, missing values, correlation patterns, and risk indicators.
- **Credit Default Prediction**: Modeling borrower default risk to assist in informed credit approval decisions.
- **Modular Architecture**: Structured for future deployment with API services and interactive monitoring dashboards.

---

## 📊 Dataset Information

This project uses the **Default of Credit Card Clients Dataset** (UCI Machine Learning Repository):
- **Instances**: 30,000 credit card clients
- **Attributes**: 24 features including financial history and demographics
- **Target Variable**: `default payment next month` (1 = Default, 0 = Non-default)

### Key Attributes:
- **Demographics**: `LIMIT_BAL`, `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`
- **Repayment Status**: `PAY_0`, `PAY_2`, `PAY_3`, `PAY_4`, `PAY_5`, `PAY_6` (repayment status across previous months)
- **Bill Amounts**: `BILL_AMT1` through `BILL_AMT6`
- **Previous Payments**: `PAY_AMT1` through `PAY_AMT6`

---

## 📁 Repository Structure

```text
CodeAlpha_credit-scoring-model/
├── api/                  # REST API endpoints (FastAPI) for real-time inference
├── dashboard/            # Interactive visualization dashboard (Streamlit)
├── data/                 # Raw and processed credit datasets
│   └── default of credit card clients.xls
├── database/             # Database connection and migration scripts
├── models/               # Serialized model weights and scalers
├── notebooks/            # Jupyter notebooks for data analysis & modeling
│   └── 01_credit_risk_eda.ipynb
├── src/                  # Core Python modules and utility functions
│   └── __init__.py
├── .gitignore            # Git exclusion rules
├── requirements.txt      # Project dependencies and libraries
└── README.md             # Project documentation
```

---

## 🚀 Getting Started

### 1. Prerequisites
Ensure you have Python 3.10+ installed on your system.

### 2. Clone the Repository
```bash
git clone https://github.com/PRANS009/CodeAlpha_credit-scoring-model.git
cd CodeAlpha_credit-scoring-model
```

### 3. Create and Activate a Virtual Environment
```bash
# On macOS/Linux:
python3 -m venv .venv
source .venv/bin/activate

# On Windows:
python -m venv .venv
.venv\Scripts\activate
```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Run the Exploratory Data Analysis Notebook
Launch Jupyter Lab or Notebook:
```bash
jupyter lab
```
Navigate to `notebooks/01_credit_risk_eda.ipynb` to inspect the dataset exploration and preprocessing workflow.

---

## 🛠️ Tech Stack

- **Language**: Python
- **Data Manipulation**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn
- **Data Source**: UCI Machine Learning Repository (`ucimlrepo`, `xlrd`)
- **Web & API Framework**: FastAPI, Streamlit

---

## 👤 Author

**Pranshu Jangra**
- GitHub: [@PRANS009](https://github.com/PRANS009)
- Repository: [CodeAlpha_credit-scoring-model](https://github.com/PRANS009/CodeAlpha_credit-scoring-model)