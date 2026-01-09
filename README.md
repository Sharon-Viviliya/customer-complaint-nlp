# customer-complaint-nlp
Customer Complaint Classification using NLP and Machine Learning
📖 Project Overview

Large organizations receive thousands of customer complaints daily. Manually categorizing these complaints is time-consuming and error-prone.
This project builds an end-to-end NLP-based classification system to automatically categorize customer complaints into predefined product categories, enabling faster ticket routing and improved customer support efficiency.

🎯 Business Problem

Unstructured complaint text makes automation difficult

Incorrect routing delays resolution

Enterprises need scalable NLP solutions

Solution:
Use Natural Language Processing (NLP) and Machine Learning to automatically classify complaints.

🧠 Problem Type

Supervised Multi-Class Text Classification

Input: Customer complaint narrative

Output: Product category

📂 Dataset

Source: Consumer Complaint Dataset (Kaggle)

Columns Used:

narrative → Complaint text

product → Target category

⚙️ Tech Stack

Language: Python

Libraries:

pandas, numpy

scikit-learn

nltk

matplotlib, seaborn

🔄 Project Pipeline

Data Loading & Cleaning

Removed null complaints

Dropped irrelevant columns

Renamed columns for clarity

Exploratory Data Analysis (EDA)

Category distribution analysis

Identified class imbalance

Text Preprocessing

Lowercasing

Removing punctuation & numbers

Stopword removal

Lemmatization

Feature Engineering

TF-IDF Vectorization

Unigrams + Bigrams

Limited to top 5000 features

Model Training

Logistic Regression (baseline & final model)

Stratified train-test split

Evaluation

Precision, Recall, F1-Score

Confusion Matrix

5-Fold Cross-Validation

Model Testing

Unseen real-world complaints

Short & ambiguous complaints

Noisy text inputs

📊 Model Performance
🔹 Test Set Results

Accuracy: 88%

Weighted F1-Score: 0.87

Macro F1-Score: 0.84

🔹 Cross-Validation

5-Fold Mean F1-Score: ~0.86

Indicates stable and generalized performance

🔍 Error Analysis

Most misclassifications occurred between semantically overlapping categories such as:

Debt Collection

Credit Reporting

🏢 Business Impact

Automates complaint routing

Reduces manual effort

Improves response time

Scales well for enterprise systems

🚀 Future Improvements

Sentence embeddings (Sentence-BERT)

Class-weight tuning for minority classes

Integration with ticketing systems (ServiceNow / Zendesk)

Feedback loop for continuous learning

📌 Author

Viviliya S
Aspiring Data Scientist | NLP & Machine Learning
