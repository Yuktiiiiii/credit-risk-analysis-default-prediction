# credit-risk-analysis-default-prediction
# Credit Risk Analysis & Credit Card Default Prediction

A machine learning project focused on predicting credit card default risk using customer demographic, credit-limit, repayment-status, billing, and payment features.

## Objective

Build and evaluate machine learning models that identify customers at higher risk of defaulting on their next credit card payment.

## Dataset

The project uses the UCI Credit Card Default dataset containing approximately 30,000 customer records and 23 original predictive features.

The target variable is `default payment next month`:
- 0 — No default
- 1 — Default

## Workflow

1. Data Cleaning
2. Exploratory Data Analysis
3. Class Distribution Analysis
4. Feature Engineering
5. Class Imbalance Analysis
6. Logistic Regression
7. Balanced Logistic Regression
8. Random Forest
9. Hyperparameter Tuning
10. Model Evaluation
11. Threshold Analysis
12. Feature Importance Analysis

## Feature Engineering

Additional features explored include:

- `has_payment_delay` — indicates whether the customer has a positive repayment-delay status
- `avg_repayment_status` — average repayment status across multiple months
- `payment_to_bill_ratio` — relationship between payment amount and bill amount

## Models

The following models were evaluated:

- Logistic Regression
- Balanced Logistic Regression
- Random Forest Classifier
- Tuned Random Forest Classifier

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

## Results

The tuned Random Forest achieved approximately:

- **ROC-AUC:** 0.779
- **Recall:** 56.2%
- **F1-score:** 54.0%
- **Accuracy:** 78.8%

The model's predictions were strongly influenced by repayment-status and payment-delay related features.

## Key Insights

- Customers with lower credit limits showed higher default rates in the dataset.
- Repayment status was an important signal for predicting default.
- Class imbalance makes accuracy alone insufficient for evaluating the model.
- Precision and recall provide useful complementary perspectives for credit-risk classification.
- Classification threshold selection involves a trade-off between identifying more potential defaults and reducing false positives.

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Future Improvements

- Perform additional feature selection and validation.
- Compare additional boosting models.
- Improve threshold selection based on business costs.
- Add model interpretability using SHAP.
- Build an interactive dashboard for risk analysis.

## Disclaimer

This project is for educational and analytical purposes and should not be used as a production credit-decision system.
