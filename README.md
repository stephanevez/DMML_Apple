
# Welcome to the Github of the **Team Apple**
This team is composed of Mael Maceiras, Stéphane Vez and Pierre Huber.

## 🔍 Project description
For the class "Data Mining & Machine Learning", which is part of our Master's programm in Information System, we were giving the following challenge:

*Real or Not? NLP with Disaster Tweets: In this project, you are challenged to build a Machine Learning model that can predict which tweets are about a real disaster and which are not. The project topic is based around a Kaggle competition.*

During the whole duration of this project, we were able to sumbmit the predictions of our model on a dedicated platform, AiCrowd. After that, it was possible to  compare our results with our pairs.


## 📅 Agenda

Under this section, you will find some information about how we proceeded during the project.

1. Week 1
* Github preparation
* Creation of our notebook
* First discovery
2. Week 2
* EDA
* First Submissions
* Reach score of 0.8134
3. Week 3
* Data Cleaning
* Hyperparameters tunning for LogReg
4. Week 4
* TF-IDF parameters tunning


## 🕵️ Solution

The solution that gave us the best accuracy was a solution using the classifier LogisticRegressionCV with a vectorizer TF-IDF. 
We reached an **accuracy score of 0.813**. We have to admit that this result was somehow disappointing as we tried many different classifiers with different parameters. However these efforts were not successful.

In the table below, it is possible to have an overview of our different tries. We can see that the **submission 6** was our winning submission.

Sub | Classifier | Tokenizer + details | test2 accuracy | score
--- | --- | --- | --- | ---
1 | LogReg(max_iter=1000) | TF-IDF default | 0.806 | 0.806
2 | LogReg(max_iter=1000) | TF-IDF default, drop.duplicates | 0.799 | 0.7819
3 | LogReg(max_iter=1000) | tokenizer=simple_preprocess | 0.793 | 0.7819
4 | LogRegCV(cv=5, max_iter=1000) | tokenizer=simple_preprocess | ? | 0.7224
5 | LogRegCV(cv=5, max_iter=1000) | tokenizer=simple_preprocess, drop.duplicate | ? | 0.7863
6 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default | x | 0.813
7 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, resampled | ? | 0.800
8 | RandomForestClassifier | TF-IDF default | 0.775 | 0.799
9 | RandomForestClassifier | TF-IDF default, resampled | ? | 0.800
10 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, merge keywords-tokens | 0.799 | 0.809
11 | LogRegCV(cv=5, max_iter=1000) | tokenizer=simple_preprocess, merge keywords-tokens | 0.806 | 0.808
12 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, improved tokens | x | 0.813
13 | LogReg(max_iter=10000) | TF-IDF default, merge keywords-tokens, hyperparams tuning: C=1.206792| x | 0.801
14 | LogReg(max_iter=10000)| TF-IDF default, merge keywords-tokens, hyperparams tuning: C=1.7575 | x | 0.8091
15 | LogReg(max_iter=10000)| TF-IDF default, hyperparams tuning: C=1.7575 | x | 0.8126
16 | LogReg(max_iter=10000)| TF-IDF default, hyperparams tuning: C=1.7575 | ? | 0.8126
17 | LogReg(max_iter=10000)| TF-IDF (ngram_range=(1, 3), min_df= 1, max_df=5.0)), C=1.206 | 0.807 | 0.8091
18 | LogReg(max_iter=10000)| TF-IDF (ngram_range=(1, 3), min_df= 1, max_df=5.0)), C=1.206, merged 'keyword' + 'text' in test df |  | 0.8038

## 📽️ Video

Here is the link to our video explaning the different steps we took for our project. Feel free to reach out if you would like any details.

In the readme.md you should a) mention the team name, b) describe the project c) your solution, and some results (using figures). d) include also a link to the video that showcases your solution.

 

