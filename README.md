# Women's Safety Analysis in Indian Cities Using ML and NLP

## What is this project about?
I built this as my final year project to address something that genuinely 
concerned me — women's safety in India. Instead of just reading about the 
problem, I wanted to quantify it using real public data.

The idea was simple: people talk about women's safety on Twitter every day. 
What if we could collect all of that, clean it up, and use machine learning 
to understand how the public actually feels about this issue across different 
cities?

## What I built
An end-to-end pipeline that collects tweets, cleans and processes the text, 
runs it through a CNN-based sentiment classifier, and displays the results 
in a desktop application built with Tkinter and MySQL.

I focused on 5 cities — Delhi, Mumbai, Pune, Chennai, and Hyderabad.

## What the results showed
The numbers were honestly striking:
- **74.6%** of tweets were negative
- **22.3%** were neutral  
- Only **3.1%** were positive

This aligned closely with a real-world survey showing 86% of working women 
in India report safety concerns — which gave me confidence that the model 
was actually capturing something real, not just noise.

## Tech stack
- **Language:** Python
- **ML/DL:** CNN, SVM, Naive Bayes (Scikit-learn)
- **NLP:** TF-IDF, text cleaning, feature extraction
- **App:** Tkinter (desktop UI), MySQL (database)
- **Data source:** Twitter (500M+ daily tweets processed)

## How to run it

```bash
# Clone the repo
git clone https://github.com/vidhisha8/womens-safety-nlp-analysis.git
cd womens-safety-nlp-analysis

# Install dependencies
pip install scikit-learn pandas numpy nltk mysql-connector-python

# Set up the database
# Import the SQL file provided in /database folder into MySQL

# Run the app
python main.py
```

## Challenges I faced
The biggest challenge was cleaning raw tweet data — slang, emojis, mixed 
languages, and abbreviations made preprocessing much harder than I expected. 
I spent a significant chunk of time just getting the text cleaning pipeline 
right before any ML could happen.

## What I'd improve
If I were to extend this, I'd add real-time Twitter API integration and 
expand to platforms like Instagram and Facebook. I'd also love to scale 
this to more cities across India.

## About me
I'm Vidhisha, a CSE(AIML) graduate from Hyderabad with a focus on AI/ML and NLP.  
Mail: vidhishamantravadi18@gmail.com  
LinkedIn: https://www.linkedin.com/in/mantravadi-vidhisha-a685013a0/
