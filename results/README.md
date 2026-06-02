# Results

This folder contains model evaluation outputs and interpretability results.

## Files

### logistic_regression_results.csv

Evaluation metrics for the Logistic Regression baseline.

### random_forest_results.csv

Evaluation metrics for the Random Forest model.

### xgboost_results.csv

Evaluation metrics for the XGBoost model.

### model_comparison.csv

Comparison table across Logistic Regression, Random Forest, and XGBoost.

### feature_selection_results.csv

Comparison of baseline Logistic Regression, LASSO, and RFECV.

### top_shap_features.csv

Top features ranked by mean absolute SHAP value.

## Main Finding

XGBoost achieved the strongest overall predictive performance, while SHAP analysis showed that inflight WiFi service, customer type, online boarding, leg room service, and arrival delay were among the most important satisfaction drivers.
