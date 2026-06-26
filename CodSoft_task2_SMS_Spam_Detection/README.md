# SMS Spam Detection - CODSOFT Task 2

A machine learning project to classify SMS messages as spam or legitimate using natural language processing techniques.

## Objective
Build a binary text classification model that can detect spam messages from legitimate ones.

## Dataset
- SMS Spam Collection Dataset
- Total messages: 5,572
- Ham (legitimate): 4,825 (86.6%)
- Spam: 747 (13.4%)

## Techniques Used
- Text Preprocessing: URL and number replacement, punctuation removal, lowercasing
- Feature Extraction: TF-IDF vectorization with unigrams and bigrams (10,000 features)
- Models trained and compared:
  - Multinomial Naive Bayes
  - Logistic Regression
  - Linear Support Vector Machine (SVM)

## Results

| Model | Accuracy | F1 Score |
|---|---|---|
| Naive Bayes | 97.3% | 0.940 |
| Logistic Regression | 98.1% | 0.960 |
| Linear SVM | 98.4% | 0.970 |

Best Model: Linear SVM with 98.4% accuracy

## Observations
- Spam messages tend to be significantly longer than legitimate messages
- Words like "free", "win", "claim", "urgent" are strong spam indicators
- All three models performed well due to the clear vocabulary difference between spam and ham
- Class imbalance (86% ham vs 14% spam) was handled using stratified train/test split

## Visualizations
- Graph 1: Spam vs Ham distribution (pie and bar chart)
- Graph 2: Message length and word count distribution
- Graph 3: Model performance comparison
- Graph 4: Confusion matrix (counts and normalised)
- Graph 5: Top spam and ham keywords
- Graph 6: ROC curves with AUC scores for all models
- Graph 7: Cross-validation F1 score boxplot

## How to Run

Install dependencies:
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

Open `sms_spam_detection.ipynb` in VS Code with the Jupyter extension installed and run all cells in order.

Note: Update the file path in Cell 1 to point to your local spam.csv location before running.

## Bonus Feature
Cell 14 allows you to type any SMS message and instantly predict whether it is spam or legitimate along with the probability score.

## Tools and Libraries
- Python 3.13
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn