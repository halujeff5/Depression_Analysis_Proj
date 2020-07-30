# AllLivesMatter-Project

Motivation: #AllLivesMatter is generally thought to be a critique or counter to the #BlackLivesMatter movement. Furthermore, there is a general misalignment and misunderstanding of the #AllLivesMatter movement. This project soughts to clarify and characterize this platform using NLP and Vader sentiment analysis of Twitter tweets with the hashtag #AllLivesMatter.

This github contains the files and ipynb notebooks necessary to reproduce my results. NOTE: these files are in the jeffng branch, NOT the master branch. The main notebooks containing my code are WorkNB_Viz.ipynb and Modeling_NB_NLP.ipynb

NECESSARY FILES:

corpus.mm, dictionary.dict, jeff.csv, WorkNB_Viz.ipynb, Modeling_NB_NLP.ipynb

PROJECT:

Vader Analysis Vader is a package especially useful on social media data that can gauge a sentiment of a piece of text from a score of -1 to 1. I used this package to successfully obtain my target variable for all my tweets. The target classes are: 'positive', 'neutral', and 'negative.'

Data Preprocessing For NLP, scraped data needed to be tokenized, stop words removed, stemmed, lemmatized and than vectorized before it can be trained in a model. Stop words removed besides English stopwords were alllivesmatter, blacklivesmatter, bluelivesmatter, twitter, http:, com, www. I did not stem the tokens, only lemmatized and used tfidf as my vectorizer.

EDA Through EDA, I created frequency distribution graphs of the words in each sentiment and created word clouds for the three sentiments as well. Also performed Latent Direlecht Allocation and made a pyLDAvis to show latent clusters in the data with their word importance in that cluster. Feature importances was also extracted from the RF model and SVM coefficients were noted (not in presentation).

Model A dummy classifier was fitted and tested first. Then Random Forest, Multinomial Naive Bayes, and SVM with a 'linear' kernel. Other kernels were fitted as well with the 'rgb' and 'linear' doing the best while 'poly' and 'sigmoid' produced predictions in the 30% range. All three models had an f1 and accuracy score of 88-90%

Conclusion #AllLivesMatter can be characterized to be a Conservative/Nationalist reactionary movement to #BlackLivesMatter. The tweet analysis shows that the messages were polarized and opinionated. With the social case established, next steps for the individual should be to investigate the message behind both sides and to sympathize for one another.
