# TASK 4: Email Spam Detection with Machine Learning

## 📌 Project Overview

This project focuses on building a **Natural Language Processing (NLP) binary classification model** that distinguishes spam messages from legitimate messages (ham). It uses text preprocessing, TF-IDF feature extraction, and machine learning algorithms to classify messages automatically.

The project demonstrates a complete text classification workflow, from data exploration and preprocessing to model training and evaluation.

## 🎯 Objectives

- Analyze the distribution of spam and ham messages.
- Clean and preprocess text data for NLP.
- Convert text messages into numerical features using **TF-IDF Vectorization**.
- Split the dataset into training and testing sets.
- Train and compare multiple machine learning classifiers.
- Evaluate model performance using classification metrics and a confusion matrix.
- Understand the importance of recall in spam detection.
- Visualize common words in spam and ham messages using WordClouds (optional).

## 🛠️ Tech Stack

- **Language:** Python
- **Environment:** Jupyter Notebook
- **Data Manipulation:** pandas, NumPy
- **Machine Learning:** scikit-learn
- **NLP and Text Processing:** NLTK, Regular Expressions (`re`)
- **Visualization:** Matplotlib, Seaborn
- **Optional Visualization:** WordCloud

## 📂 Project Structure

```text
OIBSIP/
└── Data Science/
    └── TASK-4-Email-Spam-Detection/
        ├── Email_Spam_Detection_with_Machine_Learning.ipynb
        └── README.md
        └── Spam.csv
```

## 📊 Project Workflow

### 1. Data Loading and Exploration

- Load the email/message dataset using pandas.
- Inspect the dataset structure, columns, and data types.
- Check for missing values and duplicate messages.
- Analyze spam and ham counts and percentages.

### 2. Text Preprocessing

Prepare messages for machine learning by applying text-cleaning techniques:

- Convert text to lowercase.
- Remove punctuation and unnecessary characters.
- Remove stopwords where appropriate.
- Apply stemming to reduce words to their root forms.
- Store the processed text in the `stemmed_text` column.

### 3. Feature Extraction Using TF-IDF

**Term Frequency–Inverse Document Frequency (TF-IDF)** converts text messages into numerical vectors that machine learning models can process.

It assigns higher importance to terms that are frequent in a particular message but less common across the overall collection of messages.

TF-IDF helps represent the importance of words and phrases while reducing the influence of terms that occur frequently throughout the dataset.

### 4. Train-Test Split

Split the dataset into training and testing sets:

- **Training set:** 80% of the data.
- **Testing set:** 20% of the data.
- Use stratified sampling to preserve the approximate proportion of spam and ham messages.

Fit the TF-IDF vectorizer on the training messages and use the fitted vectorizer to transform the testing messages to prevent data leakage.

### 5. Model Training

Train and compare at least two classification algorithms:

- **Multinomial Naive Bayes:** A common baseline for text classification.
- **Logistic Regression or Support Vector Machine (SVM):** An alternative classifier for comparison.

### 6. Model Evaluation

Evaluate the trained models using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of messages predicted as spam that are actually spam.
- **Recall:** Proportion of actual spam messages correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Visualizes correct and incorrect classifications.

### 7. Why Is Recall Important in Spam Detection?

Recall is important because low spam recall means that more actual spam messages are incorrectly classified as legitimate messages (ham).

A high spam recall helps identify more unwanted messages. However, precision must also be considered because incorrectly classifying legitimate messages as spam can cause important emails to be missed.

The appropriate balance depends on the application's requirements.

### 8. Optional: WordCloud Visualization

Generate separate WordCloud visualizations for spam and ham messages to explore common terms and identify potential differences in their language patterns.

## 📈 Results

The notebook evaluates the trained models using a consistent test set.

Record the actual results after running the notebook:

| Metric | Multinomial Naive Bayes | Alternative Model |
|---|---:|---:|
| Accuracy | To be measured | To be measured |
| Spam Precision | To be measured | To be measured |
| Spam Recall | To be measured | To be measured |
| Spam F1-score | To be measured | To be measured |

The final model should be selected based on the evaluation results, with particular attention to spam recall, precision, and the number of legitimate messages incorrectly flagged as spam.

## 🚀 How to Run the Project

1. Clone or download the repository.
2. Install the required libraries:

```bash
pip install pandas numpy scikit-learn nltk matplotlib seaborn jupyter
```

For the optional WordCloud visualization:

```bash
pip install wordcloud
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `Email_Spam_Detection_with_Machine_Learning.ipynb`.
5. Run the cells sequentially, starting with data loading and ending with model evaluation.

**Note:** Make sure the dataset is available at the file path specified in the notebook. If the notebook downloads NLTK resources, ensure they are available before running the preprocessing cells.

## 💡 Key Learning Outcomes

- Understanding NLP preprocessing techniques.
- Applying TF-IDF to transform text into numerical features.
- Training machine learning models for binary classification.
- Evaluating imbalanced classification problems.
- Understanding the trade-off between spam precision and recall.
- Building a reproducible machine learning workflow.

## 👨‍💻 Author

**Hazem Ebrahim**

Data Science | Machine Learning | Natural Language Processing

---

*Part of the Oasis Infobyte Internship (OIBSIP) — Data Science Track.*
