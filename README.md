# Loan Eligibility Prediction

Binary classification model predicting loan approval outcomes from applicant financial and demographic data, with comparative evaluation across five machine learning algorithms.

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn)
![Accuracy](https://img.shields.io/badge/Best%20Accuracy-87%25-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## What This Project Does

Financial institutions process thousands of loan applications manually — a slow, inconsistent process prone to human bias. This project builds and evaluates a machine learning classifier that predicts loan approval based on applicant data: income, credit history, employment status, education, and property area.

The best-performing model (**Random Forest, 87% accuracy**) provides a consistent, data-driven baseline for loan eligibility decisions.

---

## Model Performance

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
| **Random Forest** | **87%** | **0.86** | **0.87** | **0.86** |
| Gradient Boosting | 85% | 0.84 | 0.85 | 0.84 |
| Logistic Regression | 82% | 0.81 | 0.82 | 0.81 |
| SVM | 81% | 0.80 | 0.81 | 0.80 |
| Decision Tree | 78% | 0.77 | 0.78 | 0.77 |

Random Forest selected as the final model based on highest accuracy and balanced precision-recall.

---

## Key Findings

- **Credit history** is the single strongest predictor of loan approval
- Applicants with higher combined income are approved at significantly higher rates
- Graduate applicants show higher approval rates than non-graduates
- Property area (Urban / Semiurban / Rural) has a measurable but secondary effect
- Ensemble methods (Random Forest, Gradient Boosting) consistently outperform single-model approaches on this dataset

---

## ML Pipeline

```
Raw Dataset (614 records, 12 features)
          ↓
  [ Data Exploration ]      — missing value analysis, class distribution
          ↓
  [ Preprocessing ]         — null imputation, categorical encoding,
                              feature selection, train-test split
          ↓
  [ EDA ]                   — credit history impact, income distributions,
                              feature correlation analysis
          ↓
  [ Model Training ]        — 5 classifiers trained and tuned
          ↓
  [ Evaluation ]            — accuracy, precision, recall, F1-score,
                              confusion matrix per model
          ↓
  [ Final Model ]           — Random Forest (87% accuracy)
```

---

## Tech Stack

| Layer | Tools |
|---|---|
| Data Processing | Python, Pandas, NumPy |
| Machine Learning | Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |
| Version Control | GitHub |

---

## Project Structure

```
loan-eligibility-prediction/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   └── loan_eligibility_prediction.ipynb   # Full pipeline + evaluation
│
├── data/
│   └── loan_data.csv                       # Kaggle loan prediction dataset
│
└── visualizations/
    ├── credit_history_approval.png
    ├── income_distribution.png
    ├── model_comparison.png
    └── confusion_matrix_rf.png
```

---

## Setup and Usage

```bash
# Clone the repository
git clone https://github.com/asad-haris/loan-eligibility-prediction
cd loan-eligibility-prediction

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebooks/loan_eligibility_prediction.ipynb
```

---

## Dataset

**Loan Prediction Dataset** — publicly available on Kaggle  
614 records · 12 features · Binary target: `Loan_Status` (Approved / Not Approved)

Features include: Gender, Married, Dependents, Education, Self-Employed, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area.

---

## Screenshots

<img width="1189" height="821" alt="download (4)" src="https://github.com/user-attachments/assets/1c6655dc-393a-49f6-a796-76b70b73678c" />
<img width="1489" height="990" alt="download (5)" src="https://github.com/user-attachments/assets/97518673-7632-4199-a633-1232e593a062" />
<img width="1189" height="490" alt="download (7)" src="https://github.com/user-attachments/assets/5f1aaf0e-070c-46b9-ab6b-4c0afcc1bab6" />
<!-- Add 2-3 screenshots here -->
<!-- ![Model Comparison](visualizations/model_comparison.png) -->
<!-- ![Credit History Impact](visualizations/credit_history_approval.png) -->

---

## Limitations

- Dataset is relatively small (614 records) — results may not generalize to larger populations
- No real-time or live banking data; reflects historical patterns only
- Class imbalance not addressed in this version — future work could include SMOTE or class weighting
- Feature set does not include credit score, debt-to-income ratio, or repayment history, which are standard in real lending decisions

---

## License

MIT License — free to use with attribution.
