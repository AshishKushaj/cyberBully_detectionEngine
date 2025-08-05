# 🛡️ Cyberbullying Detection Web App using Machine Learning

## 📌 Introduction

With the growing influence of social media, cyberbullying has become a serious issue — especially among youth. The anonymity and reach of online platforms have created a space where harassment is easy and rampant. This project aims to combat such online abuse using **Machine Learning** and **Natural Language Processing (NLP)** to detect toxic comments in real-time and prevent their posting.

## ❌ Problem with Existing Systems

- Comment sections are open platforms for harassment.
- Existing systems **lack real-time bullying detection**.
- Previous ML attempts have shown low accuracy (~58%-61%).
- Gender-based filtering and bad word lists are insufficient and outdated.

## ✅ Proposed Solution

We present a system that:
- Uses **ML + NLP** to detect bullying comments.
- Provides a **toxicity score** and binary bullying prediction.
- Achieves **94.36% accuracy** using **Random Forest Classifier**.
- Is deployed as a web app using **Flask**.
- Enables users to check comments before posting and report abusive content.

## 🔬 Literature Survey

- Studies using Naïve Bayes, Logistic Regression, SVMs, and Random Forest were reviewed.
- Naïve Bayes showed ~75% specificity.
- Random Forest models achieved higher performance (91.6%+).
- Common preprocessing techniques like **TF-IDF**, **lemmatization**, and **tokenization** are used.

## ⚙️ Design & Architecture

### 🖥️ Requirements

**Languages & Tools:**
- Python 3.9
- Google Colab, PyCharm
- Flask (v1.1.2)

**Libraries:**
- `pandas`, `numpy`, `scikit-learn`, `scipy`
- `nltk` (Word Tokenizer, Lemmatizer, CountVectorizer, TfidfTransformer)

### 🧠 Data Flow

1. Collect → Clean → Tokenize → Lemmatize
2. TF-IDF vectorization
3. Train ML model
4. Predict bullying probability
5. Display warning or flag abusive content

## 🧩 Modules

### 📂 Dataset
- Source: [Kaggle - Cyber Troll Detection](https://www.kaggle.com/dataturks/dataset-for-detection-of-cybertrolls)
- Shape: `(20001, 3)` — tweets labeled for bullying.

### 🧼 Preprocessing
- Label extraction from JSON structure.
- Removed irrelevant columns, normalized text.
- Cleaned null values and punctuations.

### 🧪 Train-Test Split
- Split using `train_test_split` from scikit-learn.

### ✍️ NLP Techniques
- Removed non-alphanumeric chars.
- Lowercased text.
- Tokenized and lemmatized using **WordNetLemmatizer**.

### 🧮 Feature Extraction
- `CountVectorizer`: Word frequency.
- `TfidfVectorizer`: Weighted term frequency based on rarity.

### 🤖 ML Algorithms Compared
- Logistic Regression
- Naïve Bayes
- KNN
- Decision Tree
- **Random Forest** (Best Accuracy: 94.36%)

### 📊 Evaluation Metrics
- **Log-loss**
- **Hamming-loss**
- Random Forest had the lowest losses and highest accuracy.

### 🌐 Web Deployment
- Frontend: HTML, CSS, JavaScript
- Backend: Flask
- Integrated ML model (serialized with `model.pkl`)
- User pastes comment → Detects bullying → Displays result
- Optional: Report via CyberB.A.A.P portal

## 🧪 Testing & Results

- Accuracy on unseen test comment: **94.36%**
- Real-time comment tested via Web App
- Web UI lets users test & report in simple interface

## 🏁 Conclusion

This system provides a practical solution for real-time cyberbullying detection. The combination of NLP and ML has resulted in a highly accurate model. It empowers users to:
- Evaluate comments before posting.
- Report cyber abuse with confidence.

> Social media is a powerful tool — let’s use it responsibly.

## 🔮 Future Scope

- Develop as a **browser plugin** or **social media API extension**.
- Support **real-time typing analysis** (like Grammarly for toxicity).
- Improve dataset coverage with **multilingual support**.
- Extend detection to other cybercrimes (e.g., threats, scams).

## 📁 Repository

🔗 [GitHub Repository](https://github.com/Areefahnk/Web-App-Detecting-Cyber-Bullying-using-Machine-Learning)

## 📚 Bibliography

> Full reference list available in the project documentation.

Key Sources:
- [Wikipedia: Cyberbullying](https://en.wikipedia.org/wiki/Cyberbullying)
- [Kaggle Dataset](https://www.kaggle.com/dataturks/dataset-for-detection-of-cybertrolls)
- [ML Mastery Articles](https://machinelearningmastery.com/)
- [Flask Web Framework](https://opensource.com/article/18/4/flask)

---

**Let’s code to protect, not to troll. 👨‍💻🛡️**
