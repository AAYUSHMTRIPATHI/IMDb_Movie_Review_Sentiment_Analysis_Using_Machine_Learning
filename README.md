# 🎬 IMDb Sentiment Analysis using Machine Learning

## 📌 Project Overview

This project implements a complete Natural Language Processing (NLP) pipeline to classify IMDb movie reviews as **Positive** or **Negative** using classical machine learning techniques.

The objective is to demonstrate practical understanding of:

- Text preprocessing
- Feature engineering for textual data
- Machine learning model training
- Performance evaluation and comparison

---

## 📂 Dataset

- **Dataset:** IMDb 50K Movie Reviews
- **Total Samples:** 50,000 reviews
- **Classes:** Positive / Negative
- **Balanced Dataset:** Yes (25,000 positive, 25,000 negative)

Each record contains:
- Raw review text
- Sentiment label (positive or negative)

---

## 🧠 Problem Statement

Given a movie review as input, predict whether the sentiment expressed is positive or negative.

This is a **Binary Text Classification** problem.

---

## ⚙️ NLP Workflow

The complete NLP pipeline implemented in this project:

1. Raw Text Input  
2. Text Cleaning and Normalization  
3. Feature Extraction using TF-IDF  
4. Train-Test Split  
5. Model Training  
6. Model Evaluation  
7. Performance Comparison  

---

## 🧹 Text Preprocessing

The following preprocessing steps were applied:

- Conversion of text to lowercase
- Removal of punctuation, numbers, and special characters
- Stopword removal during vectorization

This ensures that the model focuses only on meaningful textual patterns.

---

## 🔢 Feature Engineering

Text data was converted into numerical format using **TF-IDF (Term Frequency – Inverse Document Frequency)**.

TF-IDF assigns higher importance to words that are meaningful within a review while reducing the weight of very common words.

The result is a high-dimensional sparse matrix representation suitable for machine learning models.

---

## 🤖 Models Implemented

### 1️⃣ Logistic Regression

- Strong baseline model for text classification
- Handles high-dimensional sparse data effectively

**Accuracy Achieved:** ~88.9%

---

### 2️⃣ Multinomial Naive Bayes

- Probabilistic model based on Bayes' Theorem
- Assumes independence between words
- Computationally efficient

**Accuracy Achieved:** ~85.2%

---

## 📊 Model Evaluation

The following metrics were used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Performance Summary

| Model                | Accuracy |
|----------------------|----------|
| Logistic Regression  | 88.9%    |
| Naive Bayes          | 85.2%    |

Logistic Regression outperformed Naive Bayes, demonstrating stronger performance on TF-IDF features.

---

## 📈 Key Insights

- Logistic Regression performs better for high-dimensional sparse text data.
- Naive Bayes provides a fast and reliable baseline model.
- Balanced dataset leads to stable evaluation metrics.
- Classical machine learning models can achieve high performance without deep learning.

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Incorporating n-grams (bigrams/trigrams)
- Comparing with ensemble methods
- Implementing deep learning models (LSTM / Transformers)
- Deploying the model using a web framework

---

## 📌 Conclusion

This project demonstrates a complete NLP sentiment classification pipeline using classical machine learning techniques. The results highlight the effectiveness of TF-IDF feature engineering combined with linear classifiers for text analysis tasks.

The implementation reflects practical understanding of NLP preprocessing, feature extraction, and model evaluation.

---

### 👤 Author  
Aayush T
