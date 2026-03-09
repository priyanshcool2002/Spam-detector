# 📧 Email Spam Classifier

End-to-end code for the **Email Spam Classifier Project**.  
Used to filter spam SMS messages using **Python and Machine Learning** with libraries like **Pandas** and **NumPy**.

---

## 📁 Project Structure

email-spam-classifier-new/

├── app.py                     # Main Streamlit application  
├── model.pkl                  # Trained MultinomialNB model  
├── vectorizer.pkl             # TF-IDF vectorizer  
├── requirements.txt           # Python dependencies  
├── nltk.txt                   # NLTK data requirements  
├── setup.sh                   # Streamlit deployment configuration  
├── sms-spam-detection.ipynb   # Complete Jupyter notebook with EDA & modeling  
├── spam.csv                   # Original dataset  
└── README.md                  # Project documentation  

---

## 🎯 How to Use

1. Enter a message in the text area  
   Example: `Congratulations! You've won a free iPhone!`

2. Click the **Predict** button

3. View the result — the app will display either:

- **Spam**
- **Not Spam**

---

## ✉️ Example Messages to Try

### Spam Examples

WINNER!! As a valued network customer you have been selected to receive  
a £900 prize reward! To claim call 09061701461.  
Claim code KL341. Valid 12 hours only.

Free entry in a 2 a wkly comp to win FA Cup final tkts 21st May 2005.  
Text FA to 87121 to receive entry question (std txt rate). T&C's apply.

### Ham Examples

Hey, are we still meeting for lunch today?

I'll be home in about 30 minutes, traffic is bad.

Did you finish the project report?

---

## 🔬 Exploratory Data Analysis (EDA)

The Jupyter notebook includes **comprehensive EDA**.

### 📊 Text Statistics

| Message Type | Avg Characters | Avg Words |
|---------------|---------------|-----------|
| Ham | 70 | 17 |
| Spam | 137 | 28 |

### 📈 Visualizations

- Word clouds for **spam and ham messages**
- Distribution plots of **message lengths**
- Correlation heatmaps
- Bar charts of **most common words**

### 🔎 Key Insights

- Spam messages tend to be **longer on average**
- Spam contains more promotional words like: **free, win, claim, cash**
- Ham messages contain more **conversational words**

---

## 🏆 Why Multinomial Naive Bayes?

Multinomial Naive Bayes was selected as the final model because:

- **High Precision (99.2%)** – critical for spam detection to avoid false positives  
- **Fast Inference** – efficient for real-time predictions  
- **Works Well with Text Data**  
- **Handles Imbalanced Data effectively**

---

## 🔮 Future Improvements

- Add support for **email attachment analysis**
- Implement **deep learning models (LSTM, Transformers)**
- Add **confidence scores** to predictions
- Create **API endpoint** for programmatic access
- Add **batch processing capability**
- Implement **user feedback mechanism**
- **Multi-language support**

---

## 📚 References

- SMS Spam Collection Dataset  
- scikit-learn Documentation  
- NLTK Documentation  
- Streamlit Documentation  

---

## 👨‍💻 Author

**Priyansh Kumar**
