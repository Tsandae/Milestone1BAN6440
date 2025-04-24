# Milestone1BAN6440
## Spam Filtering Email System Using Machine Learning Algorithm
# 📧 Spam Email Classification using Machine Learning

This project implements a spam filtering system using machine learning models trained on a labeled dataset of email messages. The goal is to classify emails as **spam** or **not spam** based on their text content.

---

## Project Overview

- **Objective:** Build a machine learning pipeline that accurately classifies emails into spam and not spam.
- **Dataset:** A CSV file with columns for `title`, `text`, and `type` .
- **Key Features:**
  - Text preprocessing (stopword removal, lemmatization)
  - Class balancing
  - TF-IDF vectorization
  - Model training (Logistic Regression, Perceptron, Linear Regression)
  - Model evaluation using accuracy and classification reports
  - Unit testing for model performance

---

## Thought Process

- Preprocess the data to remove noise and irrelevant tokens
- Balance the dataset to handle class imbalance
- Convert raw text into numerical vectors using TF-IDF
- Split the data into training and testing sets
- Train and compare multiple machine learning models
- Evaluate using accuracy, confusion matrices, and classification reports

---

## Preprocessing Steps

- Removal of subject lines, punctuation, and stopwords
- Lemmatization using WordNet
- Label encoding of `type` column (`spam` = 1, `not spam` = 0)
- TF-IDF vectorization with bigrams and max 5000 features

---

## Model Performance

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression| 0.81    |
| Perceptron         | 0.81    |
| Linear Regression  | 0.81     |

Logistic Regression performed the best with accuracy above the 0.75 threshold.

---

## Unit Testing

The `unittest` module was used to verify that all models achieved reasonable performance thresholds. All tests passed successfully.

---

## Files in the Repository
- `Milestone1BAN6440.ipynb` – Full Jupyter Notebook with all code and outputs
- `email_spam.csv` - dataset
- `README.md` – Project overview and instructions
- `Milestone1BAN6440.pptx` – Summary presentation of the project
