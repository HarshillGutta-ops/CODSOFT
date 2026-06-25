# 📱 SMS Spam Detection — CODSOFT Task 2

A machine learning project to classify SMS messages as spam or legitimate using NLP techniques.

## 📌 Objective
Binary classification — detect **spam** vs **ham (legitimate)** SMS messages.

## 📁 Dataset
- SMS Spam Collection Dataset
- Total messages: 5,572
- Ham (legit): 4,825 (86.6%)
- Spam: 747 (13.4%)

## 🛠️ Techniques Used
- **Text Preprocessing**: URL/number replacement, punctuation removal
- **Feature Extraction**: TF-IDF (unigrams + bigrams, 10k features)
- **Models Compared**:

| Model | Accuracy | F1 Score |
|---|---|---|
| Naive Bayes | ~97% | ~0.94 |
| Logistic Regression | ~98% | ~0.96 |
| Linear SVM 🏆 | ~98% | ~0.97 |

## 📊 Graphs (7 total)
- Spam vs Ham distribution
- Message length & word count distribution
- Model performance comparison
- Confusion matrix (counts + normalised)
- Top spam & ham keywords
- ROC curves with AUC scores
- Cross-validation boxplot

## 🚀 How to Run
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```
Open `sms_spam_detection.ipynb` in VS Code with Jupyter extension.

## ✨ Bonus Feature
Cell 14 lets you **type any SMS message** and instantly predict if it's spam!

## 🔧 Tools & Libraries
`Python 3.13` · `scikit-learn` · `pandas` · `numpy` · `matplotlib` · `seaborn`