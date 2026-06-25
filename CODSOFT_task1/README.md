# Movie Genre Prediction — CODSOFT Task 1

A machine learning project to predict the genre of a movie based on its plot summary using NLP techniques.

## Objective
Classify movies into one of **27 genres** using their title and plot description.

## Dataset
- Source: IMDB Genre Classification Dataset
- Training set: 54,214 movies
- Test set: 54,200 movies
- Genres: drama, comedy, documentary, thriller, horror, western, and 21 more

## Techniques Used
- **Text Preprocessing**: Lowercasing, punctuation removal, custom stopword filtering
- **Feature Extraction**: TF-IDF (unigrams + bigrams, 100k features)
- **Models Compared**:

| Model | Accuracy | F1-Weighted |
|---|---|---|
| Logistic Regression 🏆 | 60.55% | 0.575 |
| Linear SVM | 59.72% | 0.570 |
| Multinomial Naive Bayes | 55.11% | 0.483 |

## Graphs
| Graph | Description |
|---|---|
| `01_genre_distribution.png` | Distribution of 27 genres in training data |
| `02_model_comparison.png` | Accuracy & F1 comparison across 3 models |
| `03_confusion_matrix.png` | Normalised confusion matrix (top 10 genres) |
| `04_per_genre_f1.png` | Per-genre F1 score (color coded) |
| `05_top_keywords_per_genre.png` | TF-IDF keywords driving each genre |

## How to Run

### Install dependencies
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

### Run the notebook
Open `movie_genre_prediction.ipynb` in VS Code with the Jupyter extension installed.

> **Note:** Update the file paths in Cell 1 to point to your local dataset files.

## Results
- Best Model: **Logistic Regression**
- Accuracy: **60.55%**
- Strongest genres: Western (F1=0.85), Documentary (F1=0.77), Drama (F1=0.65)
- Weakest genres: Biography, History, Mystery (blend heavily into Drama)

## Tools & Libraries
`Python 3.13` · `scikit-learn` · `pandas` · `numpy` · `matplotlib` · `seaborn`
