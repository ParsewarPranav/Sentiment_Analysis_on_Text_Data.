# Sentiment Analysis on IMDb Movie Reviews 🎬🔍

## 📌 Overview
This project analyzes IMDb movie reviews and classifies them into **Positive**, **Negative**, and **Neutral** sentiments using Natural Language Processing (NLP) and Machine Learning techniques.

While the model is trained on movie reviews, this approach can be generalized for **e-commerce platforms**, **customer feedback**, and any business relying on **textual reviews**.

**Google Colab Notebook**: [Open in Colab](https://colab.research.google.com/drive/131I34j5PBuHbiC-7MBhdyR0yeSBadCDO?usp=sharing)  
**Author**: Pranav Parsewar
**LinkedIn** : https://www.linkedin.com/in/pranav-parsewar-1a8178220/

---

## 📖 Executive Summary
The project develops and evaluates machine learning models to classify IMDb reviews as **positive** or **negative**. Key components include:

- Text preprocessing
- TF-IDF feature extraction
- Classification using:
  - **Multinomial Naive Bayes**
  - **Logistic Regression**

**Best Model:** Logistic Regression  
**Accuracy:** 88.77%  
**F1 Score:** 0.89

---

## 🧠 Problem Statement
Understanding the **emotional tone** of customer reviews is critical for evaluating feedback and making data-driven decisions. This project automates sentiment classification on a large dataset of IMDb reviews.

---

## 🎯 Objective
To build an end-to-end machine learning pipeline that classifies IMDb reviews as **positive** or **negative**, and compare the performance of different models.

---

## 📂 Dataset
- Source: [Kaggle IMDb Reviews Dataset]([https://www.kaggle.com/](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews))
- Records: 50,000 pre-labelled reviews
- Labels: `positive`, `negative`, `neutral` (neutral was dropped for binary classification)

---

## 📊 Data Preprocessing
Steps included:

1. **HTML Tag Removal**
2. **Non-alphabetic Character Removal & Lowercasing**
3. **Tokenization**
4. **Stop Word Removal**
5. **Stemming** using NLTK’s `PorterStemmer`

---

## 🔎 Feature Extraction
Used **TF-IDF (Term Frequency-Inverse Document Frequency)** with `max_features=5000` to transform the cleaned text into numerical vectors.

```text
Shape of Feature Matrix: (50000, 5000)
Shape of Target Vector:  (50000,)

## Data Splitting
Data was split using an 80/20 ratio with train_test_split:

## Conclusion
This project demonstrates a complete NLP pipeline for sentiment analysis using IMDb reviews. With systematic preprocessing and model evaluation, Logistic Regression outperformed Naive Bayes and can be deployed for real-world sentiment classification tasks in industries like:

🎥 Movie recommendation

🛒 E-commerce customer review analysis

🏨 Hotel feedback processing

💬 Chatbot emotion detection



