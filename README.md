
# 🎮 Sentiment Analysis on Genshin Impact Game Reviews

This project is part of an undergraduate thesis in Data Science, focusing on sentiment analysis of user reviews for the popular role-playing game **Genshin Impact**, developed by miHoYo. With millions of players worldwide, Genshin Impact receives a wide range of user feedback — from praise for new content to criticism of game mechanics and monetization features like the gacha system. These reviews offer valuable insights into user satisfaction and expectations.

## 📌 Project Overview

- **Objective:** Analyze and classify user reviews of Genshin Impact into **positive** or **negative** sentiments using machine learning.
- **Data Source:** Preprocessed and labeled Indonesian-language reviews using a **lexicon-based approach**.
- **Key Focus:** Evaluate SVM performance on imbalanced and balanced datasets.

## 🔍 Techniques & Methodology

- **Text Preprocessing:** Cleansing, case folding, normalization, tokenizing, stopword removal, stemming
- **Feature Extraction:** TF-IDF (Term Frequency-Inverse Document Frequency)
- **Sentiment Labeling:** Based on an Indonesian sentiment lexicon
- **Modeling:** Support Vector Machine (SVM) with:
  - Linear Kernel
  - Radial Basis Function (RBF) Kernel
  - Polynomial Kernel
- **Data Balancing:** Random oversampling on the training data to address class imbalance

## 📊 Dataset Summary

- **Total Reviews:** 21,370
  - **Positive:** 14,221
  - **Negative:** 6,949
- **Data Split:**
  - Training Set: 17,096 (80%)
  - Test Set: 4,274 (20%)

## 📈 Results & Evaluation

- **Metrics Used:** Accuracy, Precision, Recall, F1-Score
- **Performance Highlights:**
  - All SVM kernels achieved **excellent** classification results (≥ 95% across all metrics)
  - **Best performance:** Linear and RBF kernels with:
    - Accuracy: 98%
    - Precision: 99%
    - Recall: 99%
    - F1-Score: 99%
  - **Polynomial kernel:** Slightly lower, but still strong performance
  - **Data balancing impact:** Minimal — SVM handled class imbalance effectively even without oversampling

## 🧪 Libraries Used

- `scikit-learn`
- `pandas`
- `numpy`
- `nltk`
- `matplotlib`, `seaborn`

## 📁 Project Structure

- `sentiment_analysis_genshin.ipynb`: Full pipeline including preprocessing, modeling, and evaluation
- `requirements.txt`: List of Python dependencies
- `data/`: *(Not included due to privacy)* — contains labeled review dataset

## 🚀 Getting Started

To run this notebook locally:

```bash
git clone https://github.com/yourusername/sentiment-analysis-genshin.git
cd sentiment-analysis-genshinimpact
pip install -r requirements.txt
jupyter notebook
```
