# Women's Safety Sentiment Analysis in Indian Cities

## About the Project

Women's safety is an important social concern in India. This project explores public discussion around women's safety by analyzing sentiment in historical Twitter data.

The project uses Python and Natural Language Processing (NLP) techniques to preprocess tweet text and classify sentiment as **Negative, Neutral, or Positive** using TextBlob polarity scores.

The objective is to examine the sentiment expressed in the available tweet dataset and present the results in a way that can help understand public discourse around women's safety.

## Project Objectives

- Analyze sentiment in historical Twitter data related to women's safety.
- Clean and preprocess text data before sentiment analysis.
- Remove punctuation, non-alphabetic tokens, and English stop words.
- Classify tweet sentiment using TextBlob polarity scores.
- Present the distribution of positive, negative, and neutral sentiment.

## Technologies Used

- **Programming Language:** Python
- **Data Processing:** Pandas, NumPy
- **Natural Language Processing:** TextBlob, NLTK
- **Data Visualization:** Matplotlib
- **Desktop Interface:** Tkinter
- **Input Data:** CSV file containing tweet text

## How It Works

### 1. Load the Dataset

The application uses a Tkinter file-selection dialog to load a CSV dataset. The supplied code reads the tweet text from a column named `Text`.

### 2. Preprocess the Text

The text-cleaning process includes:

- Splitting text into tokens.
- Removing punctuation.
- Retaining alphabetic tokens.
- Removing English stop words using NLTK.
- Removing tokens with one character or fewer.
- Converting text to lowercase and stripping surrounding whitespace.

These steps help prepare the tweet text for sentiment analysis.

### 3. Perform Sentiment Analysis

The project uses TextBlob to calculate the polarity of the text. The supplied Python code applies the following thresholds:

| Polarity score | Sentiment |
|---|---|
| Less than or equal to 0.2 | Negative |
| Greater than 0.2 and less than or equal to 0.5 | Neutral |
| Greater than 0.5 | Positive |

**Note:** The project abstract describes different threshold conditions. The table above reflects the supplied Python code; the abstract and implementation should be reconciled before presenting the thresholds as the final project methodology.

### 4. Analyze the Sentiment Distribution

The project presentation reports the following sentiment distribution:

| Sentiment | Reported percentage |
|---|---:|
| Negative | 74.6% |
| Neutral | 22.3% |
| Positive | 3.1% |

These percentages represent the distribution reported in the project presentation. They should not be interpreted as classifier accuracy or as a direct measurement of women's actual safety.

## Key Observations

The reported results show that negative sentiment accounts for the largest share of the analyzed tweet data, followed by neutral sentiment. Positive sentiment represents the smallest share.

These observations describe sentiment in the analyzed dataset only. They do not establish the actual level of safety in a city or represent the views of every person in India.

## Challenges

One of the main challenges in social media sentiment analysis is preparing text that contains inconsistent punctuation, short tokens, and other variations in informal writing. Preprocessing helps make the text more consistent before sentiment classification.

Another important consideration is that polarity-based sentiment analysis may not fully capture context, sarcasm, or the intended meaning of a tweet.

## Limitations

- The analysis depends on the contents and quality of the available CSV dataset.
- The supplied implementation uses TextBlob polarity thresholds rather than demonstrating a trained machine learning classifier.
- The supplied code does not independently verify city-wise coverage of the dataset.
- The percentages reported in the presentation have not been independently reproduced or validated here.
- Sentiment expressed in tweets is not a direct measure of real-world safety.

## Future Improvements

- Evaluate the sentiment classification against a manually labeled dataset.
- Explore machine learning and deep learning approaches and compare their performance with the current polarity-based method.
- Improve text preprocessing to handle informal language, multilingual text, and contextual expressions.
- Add verified city-wise analysis if the dataset contains reliable location information.
- Improve visualizations and reporting to make the findings easier to interpret.

## About

This project was developed as part of my final-year B.Tech academic work, focusing on Python, NLP, and the analysis of public social media text.

**Author:** Mantravadi Vidhisha

