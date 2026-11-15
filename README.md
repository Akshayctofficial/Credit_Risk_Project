# Credit Risk Project

A data science project that analyzes loan applicant data to understand and predict **credit risk**, i.e. the likelihood that a borrower will default on a loan.

> **Status:** In progress. Data inspection is complete; exploratory analysis, modeling and evaluation are planned (see [Roadmap](#roadmap)).

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Workflow](#workflow)
- [Roadmap](#roadmap)
- [Author](#author)
- [License](#license)

---

## Overview

Lenders need to decide whether an applicant is likely to repay a loan. This project works through that problem step by step, starting with a careful look at the raw data and building towards a model that predicts loan default.

**Goals**

- Understand the structure and quality of the credit risk dataset
- Identify which applicant and loan characteristics relate to default
- Build and evaluate machine learning models for default prediction

---

## Dataset

- **File:** `credit_risk_dataset.csv`
- **Size:** about 32,581 records (one row per loan applicant)
- **Content:** applicant demographics, income, employment, loan details and loan outcome

Typical columns in this dataset:

| Column | Description |
|---|---|
| `person_age` | Age of the applicant |
| `person_income` | Annual income |
| `person_home_ownership` | Rent, own, mortgage or other |
| `person_emp_length` | Employment length (years) |
| `loan_intent` | Purpose of the loan |
| `loan_grade` | Loan grade assigned |
| `loan_amnt` | Loan amount |
| `loan_int_rate` | Interest rate |
| `loan_status` | Target: 1 = default, 0 = non-default |
| `loan_percent_income` | Loan amount as a share of income |
| `cb_person_default_on_file` | Past default on record (Y/N) |
| `cb_person_cred_hist_length` | Credit history length (years) |

---

## Project Structure

```
Credit_Risk_Project/
├── 01_Data_Inspection.ipynb    # Initial data inspection and quality checks
├── credit_risk_dataset.csv     # Raw dataset
├── LICENSE                     # MIT License
└── README.md                   # Project documentation
```

---

## Tech Stack

- **Language:** Python 3
- **Libraries:** Pandas, NumPy, Matplotlib, scikit-learn
- **Environment:** Jupyter Notebook

---

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/Credit_Risk_Project.git
cd Credit_Risk_Project

# 2. (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install pandas numpy matplotlib scikit-learn jupyter

# 4. Launch the notebook
jupyter notebook 01_Data_Inspection.ipynb
```

---

## Workflow

1. **Data inspection** (done): shape, data types, missing values, duplicates and summary statistics
2. **Exploratory data analysis:** distributions, outliers and relationships with default
3. **Preprocessing:** handle missing values and outliers, encode categoricals, scale features
4. **Modeling:** Logistic Regression, Decision Tree, Random Forest and others
5. **Evaluation:** accuracy, precision, recall, F1-score, ROC-AUC and a confusion matrix

---

## Roadmap

- [x] Data inspection
- [ ] Exploratory data analysis and visualizations
- [ ] Data cleaning and feature engineering
- [ ] Baseline model (Logistic Regression)
- [ ] Advanced models and hyperparameter tuning
- [ ] Handle class imbalance
- [ ] Model comparison and final report

---

## Author

**Akshay C.T.**
AI & Data Science student, Marwadi University

- GitHub: [Akshayctofficial](https://github.com/Akshayctofficial)
- LinkedIn: [akshay-ct-8504a244a](https://www.linkedin.com/in/akshay-ct-8504a244a)

---

## License

This project is licensed under the [MIT License](LICENSE).
