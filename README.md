# 🎮 Sentiment Analysis on Genshin Impact Game Reviews

This project is a sentiment analysis of user reviews for the game **Genshin Impact**, developed as part of an undergraduate thesis in Data Science. The analysis aims to classify user opinions as **positive** or **negative** using machine learning techniques.

## 📌 Project Overview

- **Objective:** Classify game reviews based on sentiment polarity (positive/negative).
- **Data Source:** Preprocessed review dataset labeled using a lexicon-based approach.
- **Techniques Used:**
  - Text Preprocessing (cleansing, text normalization, case folding, tokenizing, remove stopwords, stemming)
  - Feature Extraction with **TF-IDF**
  - Sentiment labeling using **Indonesian lexicon-based dictionary**
  - Model training with **Support Vector Machine (SVM)** using:
    - Linear kernel
    - RBF kernel
    - Polynomial kernel
  - Class balancing using `random oversampling'`

## 📊 Dataset Summary

- Total Reviews: 21,370
- Positive: 14,221
- Negative: 6,949
- Split:
  - Training set: 17,096 reviews (80%)
  - Test set: 4,274 reviews (20%)

## 📈 Model Evaluation

- Metrics Used: Accuracy, Precision, Recall, F1-Score
- Best performance achieved by the **SVM with RBF kernel** after TF-IDF and class weight balancing.

## 🧪 Libraries Used

- scikit-learn
- pandas
- numpy
- matplotlib / seaborn (for visualization)
- nltk (for preprocessing)

## 📁 Files

- `sentiment_analysis_genshin.ipynb`: Main notebook containing full preprocessing, modeling, and evaluation.
- `requirements.txt`: Python dependencies used in this project.
- `data/`: (Not included due to privacy — contains labeled review dataset.)
- `images/`: Visualizations and graphs from the notebook.

## 🚀 Getting Started

To run this notebook locally:

```bash
git clone https://github.com/yourusername/sentiment-analysis-genshin.git
cd sentiment-analysis-genshin
pip install -r requirements.txt
jupyter notebook
