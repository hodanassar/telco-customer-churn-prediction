# IBM Telco Customer Churn Prediction
![Python](https://img.shields.io/badge/Python-3.10-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![scikit--learn](https://img.shields.io/badge/scikit--learn-ML-blue)
![XGBoost](https://img.shields.io/badge/XGBoost-Modeling-green)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-purple)
![Tableau](https://img.shields.io/badge/Tableau-Dashboard-blue)
![Business Analytics](https://img.shields.io/badge/Business-Analytics-red)

This project predicts customer churn using the IBM Telco Customer Churn dataset and translates machine learning results into actionable business insights. The goal is to identify customers who are likely to leave so the business can take preventive action through targeted retention strategies.

## Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Repository Structure](#repository-structure)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Models Used](#models-used)
- [Key Results](#key-results)
- [Risk Segmentation](#risk-segmentation)
- [Dashboard](#dashboard)
- [Tools and Technologies](#tools-and-technologies)
- [Business Recommendations](#business-recommendations)
- [Project Files](#project-files)
- [Author](#author)

## Project Overview

Customer churn is a major challenge in the telecom industry because retaining existing customers is often more cost-effective than acquiring new customers. This project uses machine learning to predict churn probability, identify key churn drivers, and segment customers into low, medium, and high risk groups.

## Objectives

- Perform exploratory data analysis on customer churn patterns
- Clean and preprocess the IBM Telco Customer Churn dataset
- Build and compare multiple classification models
- Evaluate model performance using ROC-AUC, accuracy, precision, recall, and F1-score
- Identify key churn drivers using feature importance and SHAP interpretation
- Segment customers into actionable churn risk groups
- Present insights through an executive-style Tableau dashboard

## Repository Structure

```text
telco-customer-churn-prediction/
├── notebooks/
│   └── IBM_Telco_Churn_Capstone.ipynb
├── dashboard/
│   └── README.md
├── presentation/
│   ├── Nassar_Hoda_Capstone_Presentation.pptx
│   └── Nassar_Hoda_Capstone_CoverPage_Abstract.pdf
├── data/
│   └── README.md
├── README.md
└── .gitignore
```

## Dataset

The project uses the IBM Telco Customer Churn dataset, which includes customer demographic information, account details, subscribed services, billing information, and churn status.

The dataset includes:

- 7,043 customers
- 21 features
- Churn rate of approximately 26.5%

## Methodology

The project followed a full machine learning workflow:

1. Exploratory data analysis
2. Data cleaning and preprocessing
3. Encoding categorical variables
4. Scaling numerical features where appropriate
5. Train/test split and cross-validation
6. Model development and comparison
7. Feature importance and SHAP interpretation
8. Churn probability prediction
9. Risk segmentation
10. Tableau dashboard development

## Models Used

The following classification models were developed and compared:

- Logistic Regression
- Random Forest
- Gradient Boosting / XGBoost

## Key Results

Logistic Regression achieved the strongest overall performance, with a cross-validated ROC-AUC of approximately 0.846.

The most important churn drivers included:

- Contract type
- Customer tenure
- Internet service type
- Monthly charges
- Tech support availability
- Online security availability

## Risk Segmentation

Predicted churn probabilities were converted into three customer risk groups:

| Risk Group | Churn Probability | Recommended Action |
|---|---:|---|
| High Risk | 60% or higher | Personal outreach, discount offers, contract upgrade incentives |
| Medium Risk | 30% to 60% | Targeted email campaigns, service upgrades, loyalty points |
| Low Risk | Below 30% | Standard retention, upsell opportunities, satisfaction surveys |

## Dashboard

A Tableau dashboard was created to communicate model results and business insights. The dashboard highlights churn risk segments, top churn drivers, and customer patterns related to contract type, tenure, internet service, and monthly charges.

Dashboard screenshots and notes are available in the `dashboard/` folder.

## Tools and Technologies

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- XGBoost
- SHAP
- Tableau
- Matplotlib
- Seaborn

## Business Recommendations

Based on the model results and dashboard insights, the business should:

- Prioritize retention campaigns for high-risk customers
- Focus on month-to-month customers, who showed higher churn risk
- Strengthen onboarding and engagement during the first year of customer tenure
- Investigate churn among fiber optic customers
- Offer targeted contract upgrades, loyalty incentives, or service bundles
- Use churn risk tiers to guide outreach and retention planning

## Project Files

- `notebooks/` — main Jupyter notebook
- `presentation/` — capstone presentation and abstract
- `dashboard/` — Tableau dashboard notes and screenshots
- `data/` — dataset source information

## Author

Hoda Nassar
