# CHURNGUARD AI — Customer Churn Prediction & Retention Intelligence System

## Domain
Artificial Intelligence & Machine Learning

## Project objective
Build an end-to-end supervised machine-learning workflow that analyzes historical telecom customer information and predicts whether a customer is likely to churn.

## Workflow
Raw Data → Data Understanding → Cleaning → Feature Preparation → Model Training → Evaluation → Prediction → Business Insight

## Dataset
IBM Telco Customer Churn public sample dataset.

Source:
https://github.com/IBM/telco-customer-churn-on-icp4d/blob/master/data/Telco-Customer-Churn.csv

Raw CSV:
https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv

The notebook downloads the dataset automatically in Google Colab. A local CSV can also be supplied through `LOCAL_DATA_PATH`.

## Models
1. Logistic Regression
2. Random Forest
3. Class-weighted Logistic Regression as the Day 2 improvement

## Evaluation
Accuracy, Precision, Recall, F1-score, ROC-AUC and Confusion Matrix.

The final model is selected using F1-score first, followed by Recall and ROC-AUC. Accuracy alone is not used because churn is the minority class.

## Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Google Colab / Jupyter

## Repository structure

```text
CHURNGUARD_AI/
├── CHURNGUARD_AI.ipynb
├── README.md
├── requirements.txt
├── app.py
├── PROJECT_REPORT.md
├── PROJECT_REPORT.pdf
└── evidence/
    ├── 01_churn_distribution.png
    ├── 02_churn_by_contract.png
    ├── 03_churn_by_tenure.png
    ├── 04_churn_by_monthly_charges.png
    ├── 05_confusion_matrix.png
    ├── 06_roc_curve.png
    └── 07_feature_importance.png
```

## How to run in Google Colab

1. Upload `CHURNGUARD_AI.ipynb` to Google Colab.
2. Run all cells from top to bottom.
3. The notebook downloads the IBM Telco Customer Churn CSV.
4. Review the EDA charts and model metrics.
5. Verify the Day 2 before/after comparison.
6. Confirm the final prediction and final results.
7. Download the notebook as `.ipynb`.
8. Export the project report as PDF.
9. Upload the project folder to GitHub.

## Important
Do not manually invent accuracy, precision, recall or F1 values. The notebook calculates them from the actual train/test split.
