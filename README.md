# Personalized Cancer Diagnosis Classification

## Overview
This project classifies genetic mutations in cancer based on clinical text data. Using various ML models, we aim to predict mutation classes with low log-loss by leveraging feature engineering, model tuning, and encoding techniques.

## Dataset
Data from the [MSKCC Personalized Medicine Challenge](https://www.kaggle.com/c/msk-redefining-cancer-treatment/data):
- `training_variants.csv`: Mutation details (Gene, Variation, Class).
- `training_text.csv`: Clinical text data.

## Approach
1. **Data Preprocessing**:
   - Cleaned and vectorized text using TF-IDF with unigram and bigram features.
   - Encoded categorical variables using one-hot and response encoding.

2. **Modeling**:
   - Models tested: Logistic Regression, SVM, Naive Bayes, KNN, Random Forest.
   - **Ensemble Methods**: Combined models through stacking and soft voting for potential performance gains.

3. **Evaluation**:
   - **Primary metric**: Log-loss, to capture both accuracy and confidence in predictions.
   - **Best model**: Logistic Regression with class balancing and TF-IDF, showing optimal performance based on log-loss and misclassification rate.

## Usage
1. **Run Notebook**: Open `Cancer_Diagnosis_Classification.ipynb` for full analysis and model training.

## Key Libraries
- `scikit-learn`: ML models and metrics.
- `nltk`: Text processing.
- `pandas`, `numpy`: Data manipulation.
- `matplotlib`: Visualization.

## References
- Kaggle MSKCC Challenge: [Link](https://www.kaggle.com/c/msk-redefining-cancer-treatment)
- Applied AI Course: [Link](https://www.appliedaicourse.com/)

## Acknowledgments
Inspired by Kaggle’s MSKCC Cancer Treatment Challenge and resources from the Applied AI Course. Special thanks to MSKCC for the dataset.
