# 🛡️ SpamShield XAI

**Explainable AI-Powered Email Spam Detection**

SpamShield XAI is a live, web-based email spam classifier that not only predicts whether an email is spam or ham, but also **explains why** using Explainable AI (LIME). Built with a Multinomial Naive Bayes model trained on real-world email data, this tool demonstrates the power of transparent and trustworthy AI for cybersecurity.

🌐 **Live Demo:** [SpamShield XAI on Streamlit](https://spamshieldemail-spam-detection-project-with-ai-7dj2mhwexjxbka6.streamlit.app/)

📓 **Kaggle Notebook:** [Model Training & Analysis](https://www.kaggle.com/code/mdimteyazhossen/spam-ham-emails-ditactor)

---

## 🎯 Features

- **Spam/Ham Classification:** Predicts with **98.7% accuracy** whether an email is unsolicited or legitimate.
- **Explainable AI (XAI):** Uses **LIME (Local Interpretable Model-agnostic Explanations)** to highlight which words influenced the prediction (🟢 = Safe, 🔴 = Spam).
- **Confidence Scores:** Displays probability percentages for both classes.
- **Model Insights:** Built-in expander shows classifier type, vectorizer, and confidence threshold.
- **Fully Responsive:** Custom CSS ensures a professional look on desktop, tablet, and mobile.

---

## 📸 Screenshots

| Spam Detection Result | LIME Explanation (XAI) |
|:---------------------:|:----------------------:|
| <img width="956" height="466" alt="Spam Detection Result" src="..."><br>Figure 1: Spam detection result | <img width="871" height="578" alt="LIME Explanation" src="..."><br>Figure 2: LIME explanation |

---

## 🧠 How It Works

1. **Preprocessing:** The email body is transformed into a bag-of-words vector using `CountVectorizer`.
2. **Classification:** A **Multinomial Naive Bayes** model (trained on ~5,000 emails) predicts the class and confidence.
3. **Explanation (XAI):** **LIME** perturbs the input and observes how predictions change, assigning importance scores to individual words. The result is an intuitive color-coded HTML report embedded directly in the app.

---

## 🛠️ Tech Stack

| Component               | Technology                     |
|:------------------------|:-------------------------------|
| Frontend & Backend      | Streamlit                      |
| Machine Learning        | Scikit-learn (Naive Bayes, CountVectorizer) |
| Explainable AI (XAI)    | LIME                           |
| Deployment              | Streamlit Cloud                |
| Data Processing         | Pandas, NumPy                  |

---

## 🚀 Getting Started (Run Locally)

```bash
# 1. Clone the repository
git clone https://github.com/mdimteyazhossen/SpamShield_Email-Spam-Detection-project-with-XAI-and-AI.git
cd SpamShield_Email-Spam-Detection-project-with-XAI-and-AI

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the Streamlit app
streamlit run app.py
---

## 🔒 Educational Purpose Only

This tool is developed strictly for **educational and research purposes**. It demonstrates how machine learning and explainable AI (XAI) can be applied to email spam detection. The model is trained on public datasets and is intended to raise awareness about AI interpretability in cybersecurity.

**Do not use this tool for any malicious or unlawful activities.** The developer assumes no responsibility for misuse.
