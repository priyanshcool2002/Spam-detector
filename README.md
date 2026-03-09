📧 Email Spam Classifier

An end-to-end Machine Learning project that classifies SMS messages as Spam or Not Spam (Ham).

The application is built using Python and Machine Learning and deployed using Streamlit.
It uses Natural Language Processing (NLP) techniques with TF-IDF Vectorization and a Multinomial Naive Bayes model to accurately detect spam messages.

🚀 Project Structure
email-spam-classifier-new/
│
├── app.py                       # Main Streamlit application
├── model.pkl                    # Trained MultinomialNB model
├── vectorizer.pkl               # TF-IDF vectorizer
├── requirements.txt             # Python dependencies
├── nltk.txt                     # NLTK data requirements
├── setup.sh                     # Streamlit deployment configuration
├── sms-spam-detection.ipynb     # Complete Jupyter notebook (EDA + model training)
├── spam.csv                     # Original dataset
└── README.md                    # Project documentation
🎯 How to Use

Enter a message in the text box
Example:

Congratulations! You've won a free iPhone!

Click the Predict button

The application will classify the message as:

Spam

Not Spam

🧪 Example Messages
Spam Examples
WINNER!! As a valued network customer you have been selected to receive a £900 prize reward! 
To claim call 09061701461. Claim code KL341. Valid 12 hours only.
Free entry in a weekly competition to win FA Cup final tickets. 
Text FA to 87121 to receive entry question.
Ham (Normal Messages)
Hey, are we still meeting for lunch today?
I'll be home in about 30 minutes, traffic is bad.
Did you finish the project report?
🔬 Exploratory Data Analysis (EDA)

The project includes detailed Exploratory Data Analysis in the Jupyter Notebook.

📊 Text Statistics
Message Type	Avg Characters	Avg Words
Ham	70	17
Spam	137	28
📈 Visualizations

The notebook includes:

Word clouds for spam and ham messages

Distribution plots of message lengths

Correlation heatmaps

Bar charts of most common words

🔎 Key Insights

Spam messages are generally longer.

Spam contains promotional keywords like:

free
win
claim
cash
prize

Ham messages contain normal conversational language.

🏆 Why Multinomial Naive Bayes?

Multinomial Naive Bayes was chosen because:

✔ High Precision (~99.2%) – reduces false positives
✔ Fast Prediction Speed – suitable for real-time applications
✔ Works Very Well with Text Data
✔ Handles Imbalanced Datasets Effectively

🚢 Deployment

The application is deployed using Streamlit Cloud.

Steps

Push the project to GitHub

Connect the repository with Streamlit Cloud

Configure the deployment settings

The app automatically redeploys on every push

🌐 Live Application

https://email-spam-classifier-new.streamlit.app/

🔮 Future Improvements

Possible upgrades for the project:

Email attachment analysis

Deep Learning models (LSTM / Transformers)

Prediction confidence scores

REST API for external integration

Batch message classification

User feedback system

Multi-language spam detection

📚 References

SMS Spam Collection Dataset

scikit-learn Documentation

NLTK Documentation

Streamlit Documentation

👨‍💻 Author

Priyansh Kumar
