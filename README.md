# 🛡️ Cyberbullying Detection Web App

A web app that detects toxic or bullying comments in real-time using **Machine Learning** and **Natural Language Processing (NLP)**. Built with Flask, this system achieves **94.36% accuracy** using a **Random Forest Classifier**.

---

## 📌 Overview

- Detects bullying in comments before they’re posted.
- Displays a **toxicity score** and **binary prediction**.
- Enables users to **report abusive content**.
- Deployed as a simple web interface.

---

## ❌ Problem

- Comment sections are open to harassment.
- Existing filters are outdated or inaccurate (~58–61% accuracy).
- No real-time detection in most systems.

---

## ✅ Solution

- Uses **ML + NLP** to analyze comment toxicity.
- **Random Forest** model trained with TF-IDF features.
- Provides results with **94.36% accuracy**.
- Flask backend + HTML/CSS/JS frontend.

---

## ⚙️ Tech Stack

**Languages & Tools:**
- Python 3.9
- Flask
- Google Colab / PyCharm

**Libraries:**
- `pandas`, `numpy`, `scikit-learn`, `scipy`
- `nltk` for tokenization, lemmatization, vectorization

---

## 🔄 Workflow

1. Data Collection & Preprocessing  
2. Text Cleaning, Tokenization, Lemmatization  
3. TF-IDF Vectorization  
4. Model Training (Random Forest)  
5. Real-time Prediction & UI Display

---

## 📂 Dataset

- Source: [Kaggle – Cyber Troll Detection](https://www.kaggle.com/dataturks/dataset-for-detection-of-cybertrolls)  
- Size: `20001` labeled tweets

---

## 🤖 Models Tested

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression| ~89%     |
| Naïve Bayes        | ~75%     |
| Decision Tree      | ~91%     |
| **Random Forest**  | **94.36%** ✅ |

---

## 📊 Evaluation Metrics

- **Accuracy**
- **Log-loss**
- **Hamming-loss**

---

## 🌐 Web Deployment

- Frontend: HTML, CSS, JavaScript  
- Backend: Flask (`model.pkl` for ML model)  
- User pastes comment → Model analyzes → Result displayed  
- Optional: Report abusive content via [CyberB.A.A.P portal](https://cyberbaap.in/)

---

## 🧪 Results

- **Accuracy:** 94.36% on unseen data
- Real-time testing via web UI
- Simple UX for users to test & report

---

## 🔮 Future Scope

- Browser plugin / Social media API integration  
- Typing-time analysis (like Grammarly but for toxicity)  
- Multilingual support  
- Expand detection to other cybercrimes

---

## 📚 References

- [Kaggle Dataset](https://www.kaggle.com/dataturks/dataset-for-detection-of-cybertrolls)  
- [Wikipedia: Cyberbullying](https://en.wikipedia.org/wiki/Cyberbullying)  
- [Machine Learning Mastery](https://machinelearningmastery.com/)  
- [Flask Web Framework](https://flask.palletsprojects.com/)

---

> Let’s use code to protect, not to troll. 👨‍💻🛡️
