# 📧 ML-Powered Email Classifier

An AI-based email classification system that automatically categorizes incoming emails into **Work, Personal, Spam, Promotion, or Important** using Natural Language Processing (NLP) and Machine Learning (ML).

---

## 📌 Features

- 📩 **Auto-categorizes emails** using a trained ML model (Naive Bayes)
- 🧠 Uses **TF-IDF feature extraction** on email content
- 📊 **Performance dashboard** showing:
  - Accuracy
  - Class distribution
  - Classification report
  - Confusion matrix
- 📝 **Feedback system** to correct wrong predictions (active learning)
- ♻️ Retrain model with feedback data
- 🌐 **Streamlit web app** interface

---

## 🗂 Project Structure
email_classifier_project/
│
├── app.py # Streamlit web app
├── email_classifier_nb.pkl # Trained Naive Bayes model
├── tfidf_vectorizer.pkl # TF-IDF vectorizer
├── test_data.csv # Saved test split
├── feedback.csv # Created dynamically from user feedback
└── requirements.txt # Dependencies

---
💻 Usage
📨 Classifier Tab

Paste your email content into the text box

Click Classify to get category prediction

If prediction is wrong, choose the correct label and click Submit Feedback

📊 Performance Dashboard Tab

Shows:

Accuracy of the model

Class distribution

Classification report table

Confusion matrix heatmap

Requires test_data.csv created during training.
Technologies Used

Python

Streamlit

NLTK (for text cleaning & stopwords)

Scikit-learn (TF-IDF, Naive Bayes, SVM, evaluation)

Matplotlib & Seaborn (visualization)

Joblib (model saving/loading)
Future Enhancements

Gmail API integration to fetch real emails

User authentication system

Automatic periodic retraining with feedback

---
