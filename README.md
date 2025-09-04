# 🎬 Sentiment Analysis on Movie Reviews  

This project demonstrates a complete **machine learning pipeline** for performing sentiment analysis on IMDB movie reviews. Using **Logistic Regression** with **TF-IDF features**, the model classifies reviews as either **positive** or **negative**.  

The project is designed as a **beginner-friendly introduction** to **Natural Language Processing (NLP)** and **Machine Learning** concepts.  

---

## ✨ Key Features  

- **Data Preprocessing**: Cleans raw text by removing HTML tags, punctuation, and stop words.  
- **Feature Extraction**: Converts reviews into numerical form using **TF-IDF (Term Frequency–Inverse Document Frequency)**.  
- **Model Training**: Implements a **Logistic Regression classifier** to learn sentiment patterns.  
- **Evaluation**: Provides performance metrics such as **accuracy, precision, recall, and F1-score**.  
- **Prediction**: Demonstrates sentiment prediction on new, unseen reviews.  

---

## 📂 Project Structure  

├── IMDB Dataset.csv                                   # Dataset with 50,000 reviews & sentiment labels

├── sentiment_analyzer.py                             # Core script (data loading, preprocessing, training, evaluation)

└── README.md                 # Project documentation


---

## 🚀 Getting Started  

### 🔧 Prerequisites  
- Python 3.x  
- Required libraries: `pandas`, `scikit-learn`  

### 📥 Installation & Setup  

1. **Clone the Repository**  
   ```bash
   git clone [repository_url]
   cd Sentiment-Analysis-Movie-Review
2. **Install Dependencies**
   ```bash
   pip install pandas scikit-learn
4. **Run the Script**
   ```bash
   python sentiment_analyzer.py

## ⚙️ How the Model Works

The pipeline follows a standard text classification workflow:

Data Loading: Load the IMDB dataset into a Pandas DataFrame.

**Text Preprocessing**:

   1) Convert text to lowercase

   2) Remove HTML tags, punctuation, and stop words

**Vectorization**: Use TfidfVectorizer to transform text into numerical vectors.

**Training**: Split data into training/testing sets and train a Logistic Regression model.

**Evaluation**: Test on unseen data and compute evaluation metrics.

**Prediction**: Use the trained model to classify new reviews as positive or negative.

# 📊 Example Output

**Training Progress**: Displays data preprocessing, vectorization, and model training steps.

**Evaluation Metrics**: Accuracy, precision, recall, and F1-score.

**Prediction**: Example sentiment classification on a sample review.
