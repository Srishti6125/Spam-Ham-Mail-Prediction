# 📧 Spam vs Ham Email Classifier  

## 🚀 Project Overview  
Email is a critical communication medium but is heavily exploited by spammers. Spam messages lead to phishing attacks, wasted time, and reduced productivity. Traditional rule-based filters fail to adapt to evolving spam techniques.  

This project builds a **Machine Learning (ML)-based Spam Detection System** using **Natural Language Processing (NLP)** and **Logistic Regression** to automatically classify emails as **Spam** or **Ham (Not Spam)**.  

---

## 📌 Problem Statement  
With the rise of digital communication, spam emails—ranging from ads to phishing attempts—pose serious **security and productivity challenges**. Manual filtering is inefficient, and static rules are ineffective.  
👉 This project aims to **develop a robust ML-based email classifier** that automatically detects spam with high accuracy and adaptability.  

---

## 🧩 Approach  

### 🔹 Dataset  
- A labeled dataset of emails marked as **spam (1)** or **ham (0)**.  

### 🔹 Text Preprocessing  
- Lowercasing, punctuation removal, stopword removal.  
- Lemmatization for normalization.  
- Conversion to numerical form using **TF-IDF Vectorizer** (bigrams + 5000 features).  

### 🔹 Model  
- **Logistic Regression** with balanced class weights.  
- Optimized using **precision-recall curve** to find the best classification threshold.  

### 🔹 Evaluation Metrics  
- Accuracy  
- Precision & Recall  
- Confusion Matrix  
- Precision-Recall Curve  

---

## ✅ Results & Conclusion  
- Achieved **high accuracy (>95%)** on test data.  
- Balanced **precision & recall** using optimized threshold (0.55).  
- **Advantages over rule-based filters**:  
  - Adapts to new spam trends.  
  - Reduces false positives (ham misclassified as spam).  
  - Efficient at large scale.  

---

## 🔮 Future Scope  
- Deploy as a **Streamlit/Flask web app** for real-time spam detection.  
- Integrate with **email APIs (Gmail, Outlook, etc.)** for live monitoring.  
- Experiment with **deep learning models (LSTM, BERT, Transformers)** for contextual understanding.  

---
