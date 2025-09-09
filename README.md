# Simple-Chatbot
This project implements a basic rule + machine learning hybrid chatbot using Python and scikit-learn.
It classifies user input into predefined intents (like greeting, farewell, help, etc.) and generates simple responses.

📌 Features
Text preprocessing (cleaning, lowercasing, removing special characters).
TF-IDF feature extraction with n-grams.
Intent classification using Logistic Regression.
Handles intents:
->greeting
->status_query
->name_query
->help
->weather_query
->farewell
->gratitude
Accuracy evaluation with classification report & confusion matrix.
Saves model, vectorizer, and encoder as .pkl files.
Chatbot interaction loop (works in Google Colab or local terminal).

📂 Project Structure:
├── chatbot.py                 # Main script (training + chatbot loop)
├── intent_classifier_model.pkl # Saved ML model
├── tfidf_vectorizer.pkl        # Saved TF-IDF vectorizer
├── label_encoder.pkl           # Saved label encoder
├── README.md                   # Project documentation
Installation & Setup
1. Clone the Repository
git clone https://github.com/your-username/simple-chatbot.git
cd simple-chatbot
2. Create a Virtual Environment (Optional but recommended)
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows

3. Install Dependencies
pip install -r requirements.txt
pandas
numpy
scikit-learn
matplotlib
seaborn
joblib

How It Works

1.Dataset
->A small dataset of sample user inputs (text) and corresponding intents (intent).

2.Preprocessing
->Cleans text (removes punctuation/numbers, lowercases).
->Encodes intents into numerical values.

3.Feature Extraction
->Uses TF-IDF Vectorizer with unigrams + bigrams.

4.Model Training
->Trains a Logistic Regression classifier to predict intents.

5.Evaluation
->Prints accuracy, precision, recall, F1-score.
->Plots confusion matrix.

6.Chatbot Loop
->Reads user input.
->Predicts intent.
->Returns a predefined response based on intent.

Usage:
Run Training & Chatbot:
python chatbot.py

Future Improvements
->Add more diverse dataset for better accuracy.
->Integrate weather API for live weather responses.
->Add small talk intents (jokes, casual chat).
->Deploy on Flask/FastAPI for a web-based chatbot.
->Integrate with Telegram/Discord/Slack bots.

Future Improvements:
->Add more diverse dataset for better accuracy.
->Integrate weather API for live weather responses.
->Add small talk intents (jokes, casual chat).
->Deploy on Flask/FastAPI for a web-based chatbot.
->Integrate with Telegram/Discord/Slack bots.

Project Owner:
Y. Sai Satya Bhavana
Contact:ysbhavana27@gmail.com, satyayashodayadaveni@gmail.com







