# CODSOFT Machine Learning Internship Tasks

This repository contains the work completed during the CODSOFT Machine Learning Internship. Each task involves building a machine learning model from scratch using real-world datasets, covering the complete pipeline from data preprocessing to model evaluation and visualization.

---

## Repository Structure

CODSOFT/
├── CodSoft_task1_Movie_Genre_Prediction/
│   ├── movie_genre_prediction.ipynb
│   ├── outputs/
│   └── README.md
├── CodSoft_task2_SMS_Spam_Detection/
│   ├── sms_spam_detection.ipynb
│   ├── spam.csv
│   └── README.md
├── CodSoft_task3_Customer_Churn_Prediction/
│   ├── customer_churn_prediction.ipynb
│   ├── Churn_Modelling.csv
│   └── README.md
└── README.md

---

## Task Overview

### Task 1 - Movie Genre Prediction

Built a multi-class text classification model to predict the genre of a movie based on its title and plot summary.

- Dataset: IMDB Genre Classification Dataset (54,214 movies, 27 genres)
- Techniques: TF-IDF vectorization with unigrams and bigrams
- Models: Logistic Regression, Linear SVM, Multinomial Naive Bayes
- Best Result: Logistic Regression with 60.55% accuracy
- Highlights: Western (F1=0.85) and Documentary (F1=0.77) were the strongest performing genres

| Model | Accuracy | F1-Weighted |
|---|---|---|
| Logistic Regression | 60.55% | 0.575 |
| Linear SVM | 59.72% | 0.570 |
| Multinomial Naive Bayes | 55.11% | 0.483 |

---

### Task 2 - SMS Spam Detection

Built a binary text classification model to detect spam messages from legitimate ones.

- Dataset: SMS Spam Collection Dataset (5,572 messages)
- Techniques: TF-IDF vectorization with unigrams and bigrams
- Models: Multinomial Naive Bayes, Logistic Regression, Linear SVM
- Best Result: Linear SVM with 98.4% accuracy and 0.970 F1 score
- Highlights: Includes a live prediction feature to classify any custom SMS message

| Model | Accuracy | F1 Score |
|---|---|---|
| Naive Bayes | 97.3% | 0.940 |
| Logistic Regression | 98.1% | 0.960 |
| Linear SVM | 98.4% | 0.970 |

---

### Task 3 - Customer Churn Prediction

Built a binary classification model to predict whether a bank customer will churn based on their demographics and account activity.

- Dataset: Bank Customer Churn Dataset (10,000 customers, 14 features)
- Techniques: Label encoding, standard scaling, stratified split
- Models: Logistic Regression, Random Forest, Gradient Boosting
- Best Result: Gradient Boosting with 87.1% accuracy and 0.930 ROC-AUC
- Highlights: Feature importance analysis revealed Age and IsActiveMember as the top churn indicators

| Model | Accuracy | F1 Score | ROC-AUC |
|---|---|---|---|
| Logistic Regression | 81.2% | 0.560 | 0.850 |
| Random Forest | 86.5% | 0.720 | 0.920 |
| Gradient Boosting | 87.1% | 0.740 | 0.930 |

---

## Skills Demonstrated

- Natural Language Processing (TF-IDF, text cleaning, stopword removal)
- Supervised Machine Learning (classification algorithms)
- Data Preprocessing (encoding, scaling, handling imbalanced data)
- Model Evaluation (accuracy, precision, recall, F1, ROC-AUC, cross-validation)
- Data Visualization (distribution plots, confusion matrices, ROC curves, feature importance)
- End-to-end ML pipeline development using Python

---

## Technologies Used

| Tool | Purpose |
|---|---|
| Python 3.13 | Programming language |
| scikit-learn | Machine learning models and evaluation |
| pandas | Data manipulation and analysis |
| numpy | Numerical computation |
| matplotlib | Data visualization |
| seaborn | Statistical visualizations |
| Jupyter Notebook | Development environment |

---

## How to Run Any Task

1. Clone this repository

git clone https://github.com/HarshillGutta-ops/CODSOFT.git

2. Install dependencies

pip install scikit-learn pandas numpy matplotlib seaborn

3. Open the notebook for any task in VS Code with the Jupyter extension installed

4. Update the file path in Cell 1 to point to your local dataset location

5. Run all cells in order

---

## Author

Gutta Harshill