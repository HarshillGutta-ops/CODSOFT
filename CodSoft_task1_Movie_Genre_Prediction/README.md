# Movie Genre Prediction - CODSOFT Task 1

A machine learning project to predict the genre of a movie based on its title and plot summary using natural language processing techniques.

## Objective
Build a multi-class text classification model that can classify movies into one of 27 genres using their title and plot description.

## Dataset
- Source: IMDB Genre Classification Dataset
- Training set: 54,214 movies
- Test set: 54,200 movies
- Total genres: 27 (drama, comedy, documentary, thriller, horror, western, and more)

## Techniques Used
- Text Preprocessing: lowercasing, punctuation removal, custom stopword filtering
- Feature Extraction: TF-IDF vectorization with unigrams and bigrams (100,000 features)
- Models trained and compared:
  - Logistic Regression
  - Linear Support Vector Machine (SVM)
  - Multinomial Naive Bayes

## Results

| Model | Accuracy | F1-Weighted |
|---|---|---|
| Logistic Regression | 60.55% | 0.575 |
| Linear SVM | 59.72% | 0.570 |
| Multinomial Naive Bayes | 55.11% | 0.483 |

Best Model: Logistic Regression with 60.55% accuracy

## Observations
- Western and Documentary genres had the highest F1 scores (0.85 and 0.77) due to their distinctive vocabulary
- Biography, History, and Mystery genres were harder to classify as they overlap heavily with Drama
- Combining title and description improved prediction compared to using description alone

## Visualizations
| File | Description |
|---|---|
| 01_genre_distribution.png | Distribution of all 27 genres in the training data |
| 02_model_comparison.png | Accuracy and F1 score comparison across all three models |
| 03_confusion_matrix.png | Normalised confusion matrix for the best model |
| 04_per_genre_f1.png | Per-genre F1 score with color coding |
| 05_top_keywords_per_genre.png | Most influential TF-IDF keywords for each genre |

## How to Run

Install dependencies:
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

Open `movie_genre_prediction.ipynb` in VS Code with the Jupyter extension installed and run all cells in order.

Note: Update the file paths in Cell 1 to point to your local dataset location before running.

## Tools and Libraries
- Python 3.13
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn