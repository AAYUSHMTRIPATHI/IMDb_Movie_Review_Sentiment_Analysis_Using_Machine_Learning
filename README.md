# 🎬 IMDb Sentiment Analysis using Machine Learning

## 📌 Project Overview

This project implements a complete Natural Language Processing (NLP) pipeline to classify IMDb movie reviews as **Positive** or **Negative** using classical machine learning models.

The goal is to demonstrate:

- Text preprocessing
- Feature extraction using TF-IDF
- Model training and evaluation
- Performance comparison between classifiers

---

## 📂 Dataset

- **Dataset:** IMDb 50K Movie Reviews
- **Total Reviews:** 50,000
- **Classes:** Positive / Negative
- **Balanced Dataset:** Yes (25k positive, 25k negative)

Each record contains:

- `review` → Raw review text  
- `sentiment` → Label (positive / negative)

---

## 🧠 Problem Statement

Given a movie review as input text, predict whether the sentiment expressed is:

- ✅ Positive  
- ❌ Negative  

This is a **Binary Text Classification** problem.

---

## ⚙️ NLP Pipeline
Raw Text
↓
Text Cleaning (Lowercasing + Regex Cleaning)
↓
TF-IDF Vectorization
↓
Train-Test Split
↓
Model Training
↓
Evaluation


---

## 🧹 Text Preprocessing

Steps performed:

- Convert text to lowercase
- Remove non-alphabetic characters using Regular Expressions
- Remove stopwords during vectorization

Example cleaning function:

```python
import re

def clean_text(text):
    text = text.lower()
    text = re.sub(r'[^a-zA-Z]', ' ', text)
    return text

🔢 Feature Engineering
TF-IDF Vectorization

Used TfidfVectorizer to convert text into numerical features.

Stopwords removed

Max features limited to 5000

Sparse matrix representation

TF-IDF assigns higher weights to important words while reducing the influence of common words.

🤖 Models Implemented
1️⃣ Logistic Regression

Handles high-dimensional sparse data efficiently

Strong baseline model for text classification

Accuracy: ~88.9%
F1 Score: ~0.89

2️⃣ Multinomial Naive Bayes

Based on probabilistic modeling

Assumes word independence

Fast and efficient for text data

Accuracy: ~85.2%
F1 Score: ~0.85

📊 Model Evaluation

Metrics used:

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

Logistic Regression Performance
Metric	Score
Accuracy	0.8888
F1-Score	0.89
Naive Bayes Performance
Metric	Score
Accuracy	0.8522
F1-Score	0.85

