# IMDb Movie Review Sentiment Analysis

A machine learning project that classifies IMDb movie reviews as positive or negative using Natural Language Processing, TF-IDF, and Logistic Regression.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rangga0306/movie-review-sentiment-analysis/blob/main/imdb_sentiment_analysis.ipynb)

## Project Overview

This project demonstrates an end-to-end text classification workflow, including:

- Loading and exploring the dataset
- Cleaning and preprocessing movie reviews
- Removing HTML tags, punctuation, and stop words
- Applying word stemming
- Converting text into TF-IDF features
- Training a Logistic Regression model
- Evaluating predictions using classification metrics and a confusion matrix

## Dataset

The project uses the [IMDb Dataset of 50K Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

The dataset contains:

- 50,000 movie reviews
- 25,000 positive reviews
- 25,000 negative reviews
- Two columns: `review` and `sentiment`

The dataset is downloaded automatically in the notebook using `kagglehub`.

## Model

- Algorithm: Logistic Regression
- Feature extraction: TF-IDF
- Maximum features: 5,000
- Training data: 40,000 reviews
- Testing data: 10,000 reviews
- Split ratio: 80% training and 20% testing
- Stratified split with `random_state=42`

## Results

| Class | Precision | Recall | F1-score |
|---|---:|---:|---:|
| Negative | 0.89 | 0.87 | 0.88 |
| Positive | 0.88 | 0.89 | 0.89 |

**Overall accuracy: 88.42%**

The model correctly classified 8,842 of 10,000 test reviews.

## Technologies

- Python
- pandas
- NLTK
- scikit-learn
- Matplotlib
- Jupyter Notebook
- Google Colab
- KaggleHub

## Repository Structure

```text
movie-review-sentiment-analysis/
├── README.md
├── imdb_sentiment_analysis.ipynb
└── requirements.txt
```

## How to Run

1. Open `imdb_sentiment_analysis.ipynb`.
2. Click the **Open in Colab** button.
3. Select **Runtime → Run all**.
4. The dataset will be downloaded automatically.
5. Review the evaluation results and confusion matrix.

## Limitations

- The model is designed for English-language movie reviews.
- TF-IDF does not fully capture word context or sentence meaning.
- The model may misclassify reviews containing sarcasm or ambiguous language.

## Author

**Rangga Arya Savero**  
Informatics Engineering Student focused on Data Analytics

GitHub: [@rangga0306](https://github.com/rangga0306)
