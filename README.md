# Sentiment Classification and Analysis for Tweets

Created a text classification model to identify what words are correlated with positive and negative sentiment, employing machine learning methods and data preprocessing techniques. This development involved the use of Python libraries for text cleaning, feature extraction, and model training and testing. After determining the accuracy of the model, the features found for positive and negative sentiments were used to create word clouds to further enhance the results. This project was developed within the AI4ALL Ignite accelerator.


## Problem Statement <!--- do not change this line -->

Sentiment analysis is crucial for interpreting public emotions and opinions as it transforms subjective information, such as Tweets, into actionable insights across diverse sectors. It informs business strategies by revealing customer attitudes, shapes political campaigns, enhances market research, guides crisis management, personalized user experiences, and aids investment decisions. To assist in social media monitoring and public opinion analysis, there is a need for a classification model that can accurately determine the sentiment of a customer based on the words used.

## Key Results <!--- do not change this line -->

1. Created sentiment classification model with an average accuracy of 0.79.
2. Identified what words appear most frequently for each sentiment.
      - Many of which were words typically correlated with positive and negative sentiment (i.e. *like*, *love*, *hate*, *bad*, etc.)
3. Discovered aspects that can cause prediction discrepancy.
   - Context in which the words are used in and their part of speech are important to take into account (e.x.: the difference of the word "*like*" in "I *like* apples" and in "They are *like* brothers")
   - Difficult for the model to identify emphasis of certain words in text like a human would

## Methodologies <!--- do not change this line -->

To accomplish this, we utilized a combination of techniques to build an accurate classification model that provided us with a list of words correlated with positive and negative sentiments. This project was all developed using a Python notebook in Google Collab.

#### Data Preprocessing:

We first employed the Kaggle API to retrieve the dataset containing the sample Tweets. While this dataset does contain more fields than what are mentioned, we are only concerned with the polarity representation of the tweet and the content of the tweet. This data was then cleaned using Python's text processing services, ensuring the text follows a uniform format. The data was then converted into machine-readable features using a TfidfVectorizer.

#### Machine Learning Methods:

We used the scikit-learn library to train and develop a classification model. Supervised machine learning techniques were then used to train the model on the pre-labeled dataset. The main algorithm used for developing this model was the Logistic Regression Classifier to determine the weight each feature had for each label. The overall performance of the model was evaluated by computing the main classification metrics such as precision, recall, F1 score, and accuracy based on the labels produced by the model for the testing data.

The results of this project were then further visualized by creating word clouds for both positive and negative sentiment.

## Data Sources <!--- do not change this line -->

Kaggle Datasets: (https://www.kaggle.com/datasets/kazanova/sentiment140)

## Technologies Used <!--- do not change this line -->

These are the technologies, libraries, and frameworks used in this project:
- Python
- pandas
- scikit-learn
- nltk
- Pickle
- Matplotlib
- Wordcloud

## Authors <!--- do not change this line -->

This project was completed in collaboration with:
- Paige Lee ([plee65@illinois.edu](mailto:plee65@illinois.edu))
- Shweta Narayanan ([shwetan@uw.edu](mailto:shwetan@uw.edu))
- Reva Bathula([revacb2@illinois.edu](mailto:revacb2@illinois.edu)
- Julian Alamo-Rosas([jva7@pitt.edu](mailto:jva7@pitt.edu)
  
