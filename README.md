# Twitter-Sentiment-Analysis

Objective:
The objective of our project is to use supervised machine learning models to perform sentiment analysis of tweets and classify them as negative or positive. A company or A famous personality can use this project to manage its twitter profile and can timely filter and delete the negative tweets, which in turn, can hamper its brand/reputation.

Data Description
We have collected our data from Kaggle. This data is imported in the Jupyter Notebook file by using the pandas library. The dataset contains over 600000 records and 6  columns.  Following is a small snippet of the dataset. 
![image](https://github.com/sharshil007/Twitter-Sentiment-Analysis/assets/110207080/09d8f488-781e-4121-b4d9-54c2c4bed5a1)
![image](https://github.com/sharshil007/Twitter-Sentiment-Analysis/assets/110207080/37c8c12f-612e-4e05-af76-093478e8bd9a)

Feature Engineering and Exploratory Data Analysis: 

The outcomes of machine learning algorithms vary depending on how the data are preprocessed. Therefore, the most crucial NLP activity is pre-processing. It enables us to purge all of the irrelevant information from our data and prepare it for additional processing.

a.	Removing unnecessary parts of text
In our situation, as part of the pre-processing, we have implemented a number of methods to clean our data.First, we changed the case of every tweet to lowercase. The user handle, urls, alphanumeric characters, and accent words were then taken out of the text because they didn't offer any useful information for predicting the text's sentiment.

b.	Tokenization
Next we have performed tokenization of the text. In natural language processing, tokenization is used to break down paragraphs and sentences into smaller parts so that meaning may be more easily given. We have used Tweet Tokenizer from the nltk.tokenize library to perform this task. 

c.	Removing stop words
We have removed stop words from the data as they do not provide any information and don’t contribute to decision making.We have added a function to perform this task.
Following is the function for the same.

d.	Lemmatization
In a text, different words of a tweet can have similar meaning. For example, Leafs = leaf & leaves = leaf. This is not useful. We perform lemmatization techniques to solve this problem. It is a text normalization technique that switches any word to its base root mode.
In the original dataset  for the sentiment column, “0” represented positive tweets and “4” represented negative tweets. For simplicity purpose, we have converted “4” to “1” for representing negative tweets.

Performance Evaluation and Model Comparison:
![image](https://github.com/sharshil007/Twitter-Sentiment-Analysis/assets/110207080/c33f7a9c-47d9-41f0-a35f-c13aba7ef693)
