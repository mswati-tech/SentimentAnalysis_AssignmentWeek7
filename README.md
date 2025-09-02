**Bluetooth Speaker Reviews Sentiment Analysis**

**Overview**

This project performs sentiment analysis on Bluetooth speaker reviews using Natural Language Processing (NLP) techniques. The goal is to classify reviews into Positive, Negative, or Neutral sentiments using TF-IDF features and supervised machine learning models such as Logistic Regression and Support Vector Classifier (SVC).

**Dataset**

Source: Kaggle – Bluetooth-speakers.csv

The dataset contains customer reviews for Bluetooth speakers, including a Summary column with textual feedback.

Missing values are removed during preprocessing.

**Text Preprocessing:**

Lowercasing, punctuation and number removal

Tokenization, stopword removal

Lemmatization using NLTK’s WordNetLemmatizer

**Target Labels:**

Generated using VADER sentiment analysis

Labels: Positive, Negative, Neutral

**Feature Extraction:**

TF-IDF vectorization to convert text into numerical features

Model Building

Train/Test Split: 80% training, 20% testing

**Models Trained:**

Logistic Regression (max_iter=1000)

Support Vector Classifier (SVC) with polynomial kernel because already linear fitting was used in the previous model

**Evaluation Metrics:**

Accuracy, Precision, Recall, F1-score

Confusion Matrix

Results

**Logistic Regression:**

Accuracy: 95%

Better balance in predicting Positive, Neutral, and Negative classes

**SVC:**

Accuracy: 90%

High precision for Positive class, but underpredicts Neutral and Negative

**Conclusion:** Logistic Regression outperforms SVC on this dataset due to better handling of minority classes and more balanced predictions.

Visualization

Sentiment Distribution: Bar chart showing counts of Positive, Negative, and Neutral reviews

Word Cloud: Highlights most frequent words in the review dataset

**Code script:**

25August2025.py

**Folder Structure**
bluetooth-reviews-sentiment/
│

├── Bluetooth-speakers.csv   # Dataset

├── 25August2025.py    # Python script

├── README.md                # Project description
