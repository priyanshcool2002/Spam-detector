# email-spam-classifier-new
End-to-end code for the email spam classifier project.
Used to filter spam SMS made by Python with Machine Learning using libraries like Pandas and Numpy.
email-spam-classifier-new/
│
├── app.py                 # Main Streamlit application
├── model.pkl              # Trained MultinomialNB model
├── vectorizer.pkl         # TF-IDF vectorizer
├── requirements.txt       # Python dependencies
├── nltk.txt              # NLTK data requirements
├── setup.sh              # Streamlit deployment configuration
├── sms-spam-detection.ipynb  # Complete Jupyter notebook with EDA & modeling
├── spam.csv              # Original dataset
└── README.md             # Project documentation

🎯 How to Use
Enter a message in the text area (e.g., "Congratulations! You've won a free iPhone!")

Click the "Predict" button

View the result - the app will display either "Spam" or "Not Spam"

Example Messages to Try
Spam Examples:

"WINNER!! As a valued network customer you have been selected to receivea £900 prize reward! To claim call 09061701461. Claim code KL341. Valid 12 hours only."

"Free entry in 2 a wkly comp to win FA Cup final tkts 21st May 2005. Text FA to 87121 to receive entry question(std txt rate)T&C's apply 08452810075over18's"

Ham Examples:

"Hey, are we still meeting for lunch today?"

"I'll be home in about 30 minutes, traffic is bad"

"Did you finish the project report?"

🔬 Exploratory Data Analysis (EDA)
The Jupyter notebook includes comprehensive EDA:

Text Statistics
Ham messages: Average 70 characters, 17 words

Spam messages: Average 137 characters, 28 words

Visualizations
Word clouds for spam and ham messages

Distribution plots of message lengths

Correlation heatmaps

Bar charts of most common words

Key Insights
Spam messages tend to be longer on average

Spam contains more promotional words ("free", "win", "claim", "cash")

Ham messages contain more conversational words

🏆 Why Multinomial Naive Bayes?
Multinomial Naive Bayes was selected as the final model because:

High Precision (99.2%): Critical for spam detection to avoid false positives

Fast Inference: Efficient for real-time predictions

Works Well with Text Data: Specifically designed for discrete features like word counts

Handles Imbalanced Data: Performs well despite class imbalance

🚢 Deployment
The application is deployed on Streamlit Cloud:

Push code to GitHub repository

Connect repository to Streamlit Cloud

Configure deployment settings

Deploy automatically on each push

Deployment URL: https://email-spam-classifier-new.streamlit.app/

🔮 Future Improvements
Add support for email attachments analysis

Implement deep learning models (LSTM, Transformers)

Add confidence scores to predictions

Create API endpoint for programmatic access

Add batch processing capability

Implement user feedback mechanism

Multi-language support

📚 References
SMS Spam Collection Dataset

scikit-learn Documentation

NLTK Documentation

Streamlit Documentation

👨‍💻 Author
Priyansh Kumar
