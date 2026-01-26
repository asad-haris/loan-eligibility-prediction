# Loan Eligibility Prediction using Machine Learning

## Internship Mini Project  
*Organization:* Hex Softwares Pvt. Ltd.  
*Project Type:* Data Science Internship Project  
*Difficulty Level:* Intermediate  
*Domain:* Machine Learning / Predictive Analytics  

---

## Project Overview
This project focuses on predicting **loan approval eligibility** based on applicant financial and demographic information such as income, education, employment status, credit history, and property area.

The objective is to assist financial institutions in making **data-driven, consistent, and efficient loan approval decisions** by leveraging machine learning techniques.

The project follows a **complete data science workflow**, including:
- Data Understanding
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Model Building & Evaluation
- Insights & Reporting

---

## Dataset Information
- *Source:* Kaggle – Loan Prediction Dataset  
- *Records:* 614  
- *Features:* 12  
- *Target Variable:* `Loan_Status` (Approved / Not Approved)  

The dataset contains both **categorical and numerical features**, making it suitable for classification-based machine learning tasks.

---

## Tools & Technologies
- Python 3
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- Jupyter Notebook / Google Colab

---

## 🔄 Project Workflow

### 1. Data Exploration
- Understanding dataset structure
- Identifying feature types
- Analyzing missing values
- Initial statistical summaries

---

### 2. Data Cleaning & Preprocessing
- Handling missing values
- Encoding categorical variables
- Feature selection
- Train-test data split
- Scaling where required

---

### 3. Exploratory Data Analysis (EDA)
- Loan approval distribution
- Impact of credit history
- Income vs loan approval trends
- Education and property area analysis
- Correlation analysis between features

---

### 4. Model Building
Multiple classification models were trained and evaluated:
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- Gradient Boosting

---

### 5. Model Evaluation
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score

The **Random Forest model** achieved the best overall performance and was selected as the final model.

---

## 📊 Model Performance Summary

| Model | Accuracy | Precision | Recall | F1-Score |
|------|----------|-----------|--------|----------|
| Random Forest | 87% | 0.86 | 0.87 | 0.86 |
| Gradient Boosting | 85% | 0.84 | 0.85 | 0.84 |
| Logistic Regression | 82% | 0.81 | 0.82 | 0.81 |
| SVM | 81% | 0.80 | 0.81 | 0.80 |
| Decision Tree | 78% | 0.77 | 0.78 | 0.77 |

---

## 📊 Key Insights
- **Credit History** is the strongest factor influencing loan approval
- Applicants with higher income have higher approval rates
- Graduate applicants are more likely to receive approval
- Property location has a noticeable impact on loan eligibility

---

## ⚠️ Limitations
- Dataset size is relatively small
- Data sourced from a single platform
- Does not include real-time or live banking data
- Results are dependent on historical patterns in the dataset

---

## 📝 Conclusion
This project demonstrates how machine learning techniques can be applied to automate and enhance loan eligibility decisions.  
It highlights the importance of **data preprocessing, feature selection, and model evaluation** in building reliable predictive systems.

---
