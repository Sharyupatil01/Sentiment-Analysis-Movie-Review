# Sentiment-Analysis-Movie-Review

This project demonstrates a machine learning pipeline for performing sentiment analysis on movie reviews. It uses a logistic regression model to classify a review as either positive or negative. The project is designed to be a clear and beginner-friendly introduction to natural language processing (NLP) and machine learning.

# Key Features 🔑
> Data Preprocessing: Cleans raw text data by removing HTML tags, punctuation, and common English "stop words."

> Feature Extraction: Converts text into a numerical format that a machine learning model can understand using *TF-IDF* (Term Frequency-Inverse Document    Frequency).

> Model Training: Trains a Logistic Regression classifier on the preprocessed data.

> Model Evaluation: Provides key performance metrics like accuracy, precision, and recall to assess the model's effectiveness.

> Prediction: Shows how to use the trained model to predict the sentiment of a new, unseen movie review.

#  ↗️ Project Structure 
↳ IMDB Dataset.csv: The dataset containing 50,000 movie reviews and their corresponding sentiments.

↳ sentiment_analyzer.py: The Python script that contains all the code for data loading, preprocessing, model training, and evaluation.

↳ README.md: This file, which explains the project.

#  How to Run the Project 🟡
>> Prerequisites: Make sure you have Python 3.x installed on your computer.

>> Clone the Repository: If this project is in a repository, use git clone [repository_url]. Otherwise, just make sure all the project files (the CSV file and the Python script) are in the same folder.

>> Install Dependencies: You need to install the required Python libraries. Open your terminal or command prompt and run the following command:

 >><b><i>pip install pandas scikit-learn</i></b>

>> Run the Script: Navigate to the project's directory in your terminal and execute the Python script.


>> python sentiment_analyzer.py
>> The script will print the step-by-step progress, including the model's accuracy and the final prediction on a sample review.

# How the Model Works ⚒️
The project follows a standard machine learning workflow for text classification:

<b>Data Loading </b>: The IMDB Dataset.csv is loaded into a pandas DataFrame.

<b>Text Preprocessing </b>: The raw text in the review column is cleaned. This involves converting all text to lowercase, removing unnecessary characters, and deleting common words (like 'the', 'a', 'is') that don't carry much sentiment.

<b>Vectorization </b>: The cleaned text is transformed into a numerical matrix using a TfidfVectorizer. This process turns each review into a set of numbers that represent the importance of each word within the review.

<b>Training </b>: The numerical data is split into a training set and a testing set. A Logistic Regression model is trained on the training data to learn the relationship between the words and the sentiment.

<b>Evaluation </b>: The trained model's performance is tested on the unseen data to ensure it can make accurate predictions on new reviews.

<b>Prediction</b>: The final, trained model is used to classify the sentiment of a new review, demonstrating its real-world application.
