# Explainable AI for Airline Passenger Satisfaction Analytics

This project develops and evaluates supervised machine learning models to predict airline passenger satisfaction using structured customer survey data.

The analysis compares Logistic Regression, Random Forest, and XGBoost models, then applies SHAP explainability to identify the key drivers of passenger satisfaction.

---

## Project Objective

Given demographic attributes, travel information, and airline service ratings, predict whether a passenger is:

- Satisfied
- Neutral / Dissatisfied

The project combines predictive modeling with interpretable machine learning to generate actionable business insights for airline service improvement.

---

## Dataset

The project uses the Airline Passenger Satisfaction dataset from Kaggle.

Dataset size:

- Training set: 103,904 records
- Test set: 25,976 records
- Total: 129,880 passenger survey records

Feature groups include:

- Demographics: gender, age
- Travel characteristics: customer type, travel type, class, flight distance
- Service ratings: WiFi, online boarding, seat comfort, leg room, baggage handling, cleanliness
- Operational variables: departure delay and arrival delay

---

## Methods

The project includes the following modeling workflow:

1. Data preprocessing
2. Logistic Regression baseline
3. LASSO and RFECV feature selection
4. Random Forest classification
5. XGBoost classification
6. SHAP explainability analysis

---

## Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.8715 | 0.8680 | 0.8342 | 0.8508 | 0.9256 |
| Random Forest | 0.9632 | 0.9724 | 0.9429 | 0.9574 | 0.9940 |
| XGBoost | 0.9643 | 0.9737 | 0.9441 | 0.9587 | 0.9953 |

---

## Key Findings

XGBoost achieved the strongest overall performance, with the highest accuracy, F1 score, and ROC-AUC.

SHAP analysis identified the most important drivers of passenger satisfaction:

1. Inflight WiFi Service
2. Customer Type
3. Online Boarding
4. Leg Room Service
5. Arrival Delay in Minutes

These results suggest that airlines can improve customer satisfaction by prioritizing digital service quality, loyalty program design, boarding experience, cabin comfort, and on-time performance.

---

## Repository Structure

```text
.
├── data/
│   └── README.md
│
├── docs/
│   └── Final_Project_Report.pdf
│
├── figures/
│   ├── model_performance_comparison.png
│   ├── shap_summary_plot_original.png
│   ├── feature_importance.png
│   └── preprocessing_pipeline.png
│
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_logistic_regression_baseline.ipynb
│   ├── 03_feature_selection_rfecv.ipynb
│   ├── 04_random_forest_model.ipynb
│   ├── 05_xgboost_model.ipynb
│   ├── 06_shap_explainability.ipynb
│   ├── original_project_code.ipynb
│   └── README.md
│
├── results/
│   ├── logistic_regression_results.csv
│   ├── random_forest_results.csv
│   ├── xgboost_results.csv
│   ├── model_comparison.csv
│   ├── feature_selection_results.csv
│   ├── top_shap_features.csv
│   └── README.md
│
├── requirements.txt
└── README.md
```

---

## Tools

- Python
- Pandas
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib

---

## Author

Yunxuan (Ariel) Hu  
M.S. Business Analytics  
University of Arizona
