# 📩 SMS Spam Detection ML App

This is a **Machine Learning project** that classifies SMS messages as **Spam** or **Not Spam**.  
The app uses **TF-IDF feature extraction** and a **high-precision ML model** to ensure reliable spam detection.

---

## 🧠 Problem Statement

SMS spam is a common issue that can be annoying or even dangerous.  
This project builds an ML model to automatically detect spam messages while **minimizing false positives**.

---

## ⚡ Features

- Predicts whether an SMS message is **Spam** or **Not Spam**  
- High-precision model for **reliable predictions**  
- Web app built using **Streamlit**  
- Easy to test and deploy

---

## 🛠 Tech Stack

- **Language:** Python  
- **ML Library:** scikit-learn  
- **Web App:** Streamlit  
- **Data Processing:** Pandas, NumPy  
- **Model:** Multinomial Naive Bayes (optimized for high precision)  
- **Vectorizer:** TF-IDF

---

## 🧪 Model Performance

| Metric       | Value |
|--------------|-------|
| Accuracy     | 97%   |
| Precision    | 98%   |
| Recall       | 81%   |

> The model is optimized for **high precision** to avoid false spam alerts.

---

## 📝 Jupyter Notebook (`notebook/sms_spam_detection.ipynb`)

The notebook contains the **complete development workflow** of the SMS Spam Detection project:

1. **Data Loading & Exploration (EDA)**  
   - Loaded SMS dataset  
   - Checked class distribution (spam vs ham)  
   - Performed basic text analysis (message lengths, word counts)

2. **Data Preprocessing**  
   - Lowercased text  
   - Removed punctuation  
   - Tokenized and cleaned messages  

3. **Feature Extraction**  
   - Converted text into **numerical features using TF-IDF**  
   - Experimented with `max_features` to balance precision and recall  

4. **Model Building & Evaluation**  
   - Trained **Multinomial Naive Bayes** and other ML model (Logistic Regression)  
   - Compared metrics: **accuracy, precision, recall**  
   - Selected **high-precision model** for deployment  

5. **Pickle Export**  
   - Saved trained model and TF-IDF vectorizer using `pickle`  
   - Used these files for deployment in the Streamlit app  

6. **Conclusion**  
   - Explained trade-offs between precision and recall  
   - Justified model selection based on real-world spam detection requirements

[View Full Notebook](notebook/sms_spam_detection.ipynb)

---

## 📂 File Structure

 ms-spam-classifier/
│
├── app.py # Streamlit web app
├── model.pkl # Trained ML model
├── tfidf.pkl # TF-IDF vectorizer
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── .gitignore # Ignored files/folders
└── notebook/
       └── sms_spam_detection.ipynb # Jupyter notebook with EDA and experiments


---

## 🚀 How to Run Locally

1. Clone the repo:

```bash
git clone https://github.com/ankitkumar6507/sms-spam-classifier.git
cd sms-spam-classifier
pip install -r requirements.txt
streamlit run app.py
    
