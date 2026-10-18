# Women's Safety Sentiment Analysis in Indian Cities (NLP & ML)

## What is this project about?
I built this as my final-year project to address an issue that genuinely concerns me — women's safety in India. Instead of just reading about the problem, I wanted to analyze public discourse around it using real-world social media data.

People discuss women's safety on Twitter/X every day. The goal of this project is to take historical public tweet datasets, clean the noisy text, and apply Natural Language Processing (NLP) and Machine Learning classifiers to quantify public sentiment across major Indian cities.

## What I built
An end-to-end desktop application built with **Python (Tkinter)** and **MySQL** that:
1. Ingests curated Twitter datasets covering 5 major Indian cities — **Delhi, Mumbai, Pune, Chennai, and Hyderabad**.
2. Applies an automated NLP preprocessing pipeline (lowercasing, punctuation/URL removal, stop-word removal using **NLTK**, and **TF-IDF** feature extraction).
3. Trains and compares Machine Learning and Deep Learning classifiers (**SVM, Naive Bayes, and CNN**) to classify tweets into Positive, Negative, or Neutral categories.
4. Stores processed records in a **MySQL** relational database and visualizes sentiment distribution charts directly in the GUI.

## Key Findings
Across the evaluated urban tweet dataset, the classification results highlighted a stark trend:
* **74.6%** of discourse was classified as **Negative**
* **22.3%** was classified as **Neutral**
* **3.1%** was classified as **Positive**

These findings align closely with national survey data indicating that up to 86% of working women in India report safety concerns in urban transit and public spaces.

## Tech Stack
* **Programming Language:** Python
* **Data Processing & NLP:** Pandas, NumPy, NLTK (Stopwords, Tokenization), Scikit-Learn (TF-IDF Vectorizer)
* **Machine Learning / Deep Learning:** Scikit-Learn (SVM, Naive Bayes), Keras / TensorFlow (CNN Classifier)
* **Frontend / GUI:** Tkinter (Python Desktop GUI)
* **Database:** MySQL (`mysql-connector-python`)
* **Data Source:** Offline Curated Twitter Dataset (CSV)

## How to Run Locally

# 1. Clone the repository
git clone https://github.com/vidhisha8/womens-safety-nlp-analysis.git
cd womens-safety-nlp-analysis

# 2. Install required dependencies
pip install scikit-learn pandas numpy nltk tensorflow matplotlib mysql-connector-python

# 3. Set up the MySQL Database
# Open MySQL Workbench or CLI and import the SQL schema located in the /database folder

# 4. Run the Tkinter application
python main.py

## Challenges I Faced
The biggest challenge was cleaning raw social media text. Tweets contain slang, emojis, URLs, @mentions, mixed languages (Hinglish), and inconsistent punctuation. Getting the regex cleaning, stop-word filtering, and TF-IDF vectorization pipeline right was critical before feeding the features into the classification models.

## Future Improvements
* Transition the desktop Tkinter UI to a web-based **Django** or **Streamlit** dashboard.
* Integrate live social media scraping / API streaming for real-time trend monitoring.
* Experiment with transformer-based models (like BERT or LLM APIs) to better capture sarcasm and bilingual context.

## About Me
I'm **Mantravadi Vidhisha**, a B.Tech CSE (AI & ML) graduate from Hyderabad passionate about Python development, SQL, and applied AI/NLP.
* **Email:** vidhishamantravadi18@gmail.com
* **LinkedIn:** https://www.linkedin.com/in/mantravadi-vidhisha/
