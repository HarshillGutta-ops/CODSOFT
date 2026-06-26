# Customer Churn Prediction - CODSOFT Task 3

A machine learning project to predict customer churn for a subscription-based business using historical customer data and demographic features.

## Objective
Build a binary classification model to identify customers who are likely to leave the service, enabling the business to take proactive retention measures.

## Dataset
- Bank Customer Churn Dataset (Churn_Modelling.csv)
- Total customers: 10,000
- Features: 14 (demographics, account info, activity)
- Churned: 2,037 (20.4%)
- Retained: 7,963 (79.6%)

## Features Used
- CreditScore, Geography, Gender, Age, Tenure
- Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary

## Techniques Used
- Label Encoding for categorical features (Geography, Gender)
- Standard Scaling for Logistic Regression
- Stratified Train/Test Split (80/20)
- Models trained and compared:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting

## Results

| Model | Accuracy | F1 Score | ROC-AUC |
|---|---|---|---|
| Logistic Regression | 81.2% | 0.560 | 0.850 |
| Random Forest | 86.5% | 0.720 | 0.920 |
| Gradient Boosting | 87.1% | 0.740 | 0.930 |

Best Model: Gradient Boosting with highest ROC-AUC score

## Observations
- Age is the most important feature - older customers churn more
- Inactive members are significantly more likely to churn
- Customers from Germany have a higher churn rate than France and Spain
- Customers with only one product are more likely to leave
- High balance customers with low activity are high churn risk

## Visualizations
- Graph 1: Churn distribution (pie and bar chart)
- Graph 2: Feature distributions by churn status
- Graph 3: Model performance comparison (Accuracy, Precision, Recall, F1, ROC-AUC)
- Graph 4: Confusion matrix (counts and normalised)
- Graph 5: ROC curves with AUC scores for all models
- Graph 6: Feature importance from Random Forest
- Graph 7: Feature correlation heatmap
- Graph 8: Cross-validation ROC-AUC boxplot

## How to Run

Install dependencies:
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

Open `customer_churn_prediction.ipynb` in VS Code with the Jupyter extension installed and run all cells in order.

Note: Update the file path in Cell 1 to point to your local Churn_Modelling.csv location before running.

## Bonus Feature
Cell 14 allows you to input any customer details and instantly predict their churn probability.

## Tools and Libraries
- Python 3.13
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn