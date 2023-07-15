# Restaurant-Review-by-NLP
Project classifying Natural Language Review Dataset of a Restaurant into positive (1) and negative (0).
Uses Pandas, Natural Toolkit (NLTK) and Sklearn libraries.
Dataset Collected from Kaggle. Link - https://www.kaggle.com/datasets/d4rklucif3r/restaurant-reviews

This Dataset contains two rows Customer Reviews and Liked.
Customer reviews tells us about the reviews given by the customers for a food in restaurant and liked column tells about whether they liked the food or not.

Comprehension of tasks involved
1. A csv file is given. The csv file contains reviews and '1' or '0' based on positive and negative reiews as comma seperated values. So we use delimiter as \t. 
2. We preprocess the text and remove any punctuations, numbers using the nltk.corpus.stopwords module.
3. To stem the words to their rootwords, we use StemmerPorter module from nltk.stem.porter.
4. We tokenize the sentences into words and make a bag of words via sparse matrix which can be achieved by sklearn.feature_extraction.text.CountVectorizer.
5. We then convert the corpus into an array. If the review is positive it will store '1' in the adjacent column else it will store '0' if it is false.
6. Train and test the data using train_test_split() from sklearn.cross_validation library.




