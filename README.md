# Quora-Questions-Pairs-Similarity-Problem
 Identify which questions asked on Quora are duplicates of questions that have already been asked. This could be useful to instantly provide answers to questions that have already been answered. We are tasked with predicting whether a pair of questions are duplicates or not. Used TF-IDF, logistic regression, SVM, XGBoost etc.

# Procedure and Observation
1) First we did Exploratory Data Analysis on Quora Question Pair data in which we performed such as finding number of different questions, checking for duplicates, number of occurence of questions etc. 
2) Then we performed some feature extraction like fuzz ratio, fuzz partial ration, longest common substring etc. 
3) After performing feature extraction we applied some visualisation techniques such as pair-plot, violin plot, TSNE etc. 
4) Then we peformed tfidf-w2vec vectorizer on pair of questions dataset and then we merged each tfidf-w2vec vectors to our advanced featured vectors. 
5) In the next step we applied some machine learning algorithm such as logistic regression, support vector machines etc and found log-loss for both train and test dataset. 
6) After choosing best parameters we then plotted confusion matrix, precision matrix and recall matrix for each one. 
7) We did same process for tfidf vectorizer at the end of this project.

+---------------------+-------------+----------+
|        Model        |  vectorizer | log loss |
+---------------------+-------------+----------+
| Logistic regression | TFIDF w2vec |  0.5651  |
|      Linear SVM     | TFIDF w2vec |  0.5362  |
|       XGBOOST       | TFIDF w2vec |  0.3896  |
| Logistic regression |    TFIDF    |  0.5001  |
|      Linear SVM     |    TFIDF    |  0.5025  |
|       XGBOOST       |    TFIDF    |  0.3396  |
+---------------------+-------------+----------+


