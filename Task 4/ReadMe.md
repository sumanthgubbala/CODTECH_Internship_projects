**Intern:** Sumanth Gubbala  
**Intern ID:** CT12RAU  
**Company:** CodTech IT Solutions  
**Mentor:** Sravani  
**Duration:** 8 Weeks

## 4️⃣ Sentiment Analysis (IMDb Reviews - NLP) 

# 🎬 IMDb Movie Review Sentiment Analysis

## 📌 Project Overview
This project focuses on analyzing sentiment from IMDb movie reviews using **TF-IDF vectorization** and **Logistic Regression**. The model is trained to classify reviews as **Positive** or **Negative** based on textual content. This is a practical application of **Natural Language Processing (NLP)** for understanding audience feedback on movies.

---

## 📝 Description

### **🔹 Problem Statement**
Sentiment analysis is widely used in **opinion mining** for analyzing customer feedback, social media posts, and product reviews. In this project, we analyze **IMDb movie reviews** to determine whether they express a **positive** or **negative** sentiment.

### **🔹 Dataset**
- **Source:** IMDb Reviews Dataset (Kaggle)
- **Size:** 50,000 movie reviews
- **Labels:** "Positive" (1) and "Negative" (0)

---

## 🚀 Project Workflow

### **Step 1: Data Preprocessing**
✔ Convert text to **lowercase**  
✔ Remove **HTML tags, special characters, and stopwords**  
✔ Apply **TF-IDF vectorization** to convert text into numerical form  

### **Step 2: Model Training**
- The dataset is split into **80% training** and **20% testing**.
- **TF-IDF features** are extracted from the cleaned text.
- **Logistic Regression** is used for classification.

### **Step 3: Model Evaluation**
The trained model is evaluated using:
- **Accuracy Score**: Measures the overall correctness of predictions.
- **Precision, Recall & F1-score**: Measures classification performance.
```
  Model Accuracy: 0.8891
              precision    recall  f1-score   support

           0       0.90      0.87      0.89      4961
           1       0.88      0.90      0.89      5039

    accuracy                           0.89     10000
   macro avg       0.89      0.89      0.89     10000
  weighted avg       0.89      0.89      0.89     10000
```
### **Step 4: Prediction System**
A function is implemented to classify new movie reviews using the trained model.

```python
def predict_sentiment(review, model, vectorizer):
    cleaned_review = preprocess_text(review)  # Clean the text
    review_tfidf = vectorizer.transform([cleaned_review])  # Convert to TF-IDF
    prediction = model.predict(review_tfidf)
    return "Positive" if prediction[0] == 1 else "Negative"
```

## **📌 Output Screenshots**

![image](https://github.com/user-attachments/assets/c710bd49-1b2d-4317-9e8a-b2b8442e3bc6)

