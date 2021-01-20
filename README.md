<<<<<<< HEAD
# Depression_Analysis_Proj
Project to predict depression in individuals by doing NLP on their tweets

This project is about predicting depression in social media tweets. The application of this project us to detect depression in individuals based on their tweet history. Using LIWC, a pyscholinguistic vocabulary package, I was able to assess a given level of pychological processes in a tweet. Sadness was the emotion I chose to measure with LIWC to give me indications of depression in subject's tweets. After labeling 130,000 tweets as depressed or not, I used NLP to conduct EDA and predict a testing set to arrive at model evaluations. The class balance of the tweets were 114580 not depressed and 6198 depressed.

Below is a word cloud describing words from the two catagories.

Not depressed word cloud
![Screen Shot 2020-10-02 at 9 33 57 AM](https://user-images.githubusercontent.com/59067730/94929920-b5b25900-0493-11eb-9bad-ac4d546a49f0.png)

Depressed word cloud
![Screen Shot 2020-10-02 at 9 51 08 AM](https://user-images.githubusercontent.com/59067730/94931065-4d647700-0495-11eb-8819-68af54a35abe.png)


Upsampling was done to account for class imbalance and the best model obtained was the Logistic Regression model which predicted depression up to a 86% accuracy/F1/recall. The multinomial Naive Bayes fared second with an 80% accuracy/F1/recall.

With a 86% F1/recall/accuracy score this model can be used in conjunction with other pyschological diagnostics to predict depression in individuals. Recall is important in our case because it gives us the rate where depression is not predicted when in fact there is. This metric is called false negatives and failure to address this would mean individuals are not being diagnosed when in fact they do suffer from depression. These individuals will not be getting any treatment for their condition under this circumstance.

A Flask front-end interface where the user can input description of how he/she is feeling that day, and have diagnostic of 'depression' or not and a overall score, will be deployed soon.  
||||||| empty tree
=======
# Depression_Analysis_Proj
Project to predict depression in individuals by doing NLP on their tweets. Using LIWC a sentiment recognition library, I was able to detect sadness in tweets and than give it a numerical rating. I than separated the ratings to >5 (sadness present) and categorized the dependent variable to depressed and not depressed. From there, I conducted NLP on the tweets and trained several ML model to test if I could predict 'depressed' or 'not depressed' based on the language on their tweets. The models I used were Multinomial Naive Bayes, SVM, Logistic Regression, Random Forest. The Logistic Regression model fared best with a 85% F1 score.

Further developments for this model include acheiving a higher F1 score with more robust data. We can ask professional psychiatrists the threshold for the sadness score that would indicate depression. And definitely using different social media platforms such as facebook would be more accurate since these posts tend to be longer. This model serves its purpose as a depression diagnostic tool if social media posts (tweets) are measured for a period of time with the same individual. It is easy to employ and gives fairly reliable results.  
>>>>>>> f36768fd20733d81d9724415b4eeee0655b1f410
