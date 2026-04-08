# SMS Spam Detection — NLP Text Classification

Binary text classifier to detect spam SMS messages using TF-IDF and Logistic Regression.

## Overview
This project builds a spam detection pipeline on 5,572 SMS messages, comparing different preprocessing approaches and evaluating model performance.

## What's covered
- Text cleaning and preprocessing
- Tokenization, stopword removal and lemmatization (NLTK)
- TF-IDF vectorization with bigrams
- Logistic Regression with class balancing
- Comparison of clean text vs lemmatized text as features
- Overfitting check — train vs test accuracy comparison

## Dataset
[SMS Spam Collection](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset) via Kaggle — 5,572 labelled SMS messages (ham/spam).

## Results
- 98.4% accuracy using clean text + TF-IDF + bigrams
- Ham: 99% precision, 99% recall
- Spam: 95% precision, 92% recall

## Key findings
- Clean text outperformed lemmatized text (98.4% vs 97.8%) — spam vocabulary is distinctive enough that lemmatization adds no value
- Bigrams capture strong spam signals like "free entry", "win prize" and "call now"
- No overfitting — train accuracy 99.2% vs test accuracy 98.4%

## Libraries
- pandas, numpy
- nltk
- scikit-learn

## Author
GreenBlueberryKate
