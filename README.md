
# Welcome to the Github of the **🍏Team Apple🍏**
This team is composed of Mael Maceiras, Stéphane Vez and Pierre Huber.

## 🔍 Project description
For the class "Data Mining & Machine Learning", which is part of our Master's programm in Information System, we were giving the following challenge:

*Real or Not? NLP with Disaster Tweets: In this project, you are challenged to build a Machine Learning model that can predict which tweets are about a real disaster and which are not. The project topic is based around a Kaggle competition.*

During the whole duration of this project, we were able to submit the predictions of our model on a dedicated platform, AiCrowd. After that, it was possible to  compare our results with our pairs.

## 🦮 Guidance

Our repository is organised in 3 folders.
* Documents
* Code
* Data

### Documents
Under this folder, you will find additional docs in relation with this project.

### Code
This folder stores our different Notebooks we developped during this challenge. We decided to separe our code in different Notebooks in order to improve the readability and speed of excecution.
* Apple_FinalSub.ipynb : contains our model with the best accuracy.
* Apple_EDAandProcessing.ipynb : contains everything related to our EDA as well as the preprocessing of the data. From this notebook results a new dataset "training_preprocessed".
* Apple_Results.ipynb : contains all the different tries and submissions we did during this challenge.

### Data
In the folder "Data", you can find the data that was provided for this challenge as well as our dataset "training_preprocessed".

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
* Final preparations

## 🕵️ Solution

The solution that gave us the best accuracy was a solution using the classifier LogisticRegressionCV (CV = 5, max_iter = 1000) with a vectorizer TF-IDF (default parameters). 
We reached an **accuracy score of 0.813**. We have to admit that this result was somehow disappointing as we tried many different classifiers with different parameters. However these efforts were not successful.

In the table below, it is possible to have an overview of our different tries. We can see that the **submission 6** was our winning submission.

Sub | Classifier | Tokenizer + details | test_split accuracy | score
--- | --- | --- | --- | ---
1 | LogReg(max_iter=1000) | TF-IDF default, Simple Tokenizer | 0.806 | 0.806
2 | LogReg(max_iter=1000) | TF-IDF default, duplicates dropped | 0.799 | 0.7819
3 | LogReg(max_iter=1000) | TF-IDF default, Tokenizer = SimplePreprocess | 0.793 | 0.7819
4 | LogRegCV(cv=5, max_iter=1000) | Tokenizer = SimplePreprocess | ? | 0.7224
5 | LogRegCV(cv=5, max_iter=1000) | Tokenizer = SimplePreprocess, duplicates dropped | ? | 0.7863
6 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, Simle Tokenizer | x | 0.813
7 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, Simple Tokenizer, Resampled | ? | 0.800
8 | RandomForestClassifier | TF-IDF default, Simple Tokenizer | 0.775 | 0.799
9 | RandomForestClassifier | TF-IDF default, Simple Toenizer, Resampled | ? | 0.800
10 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, merge keywords-tokens | 0.799 | 0.809
11 | LogReg(max_iter=1000)| TF-IDF default, merge keywords-tokens | 0.806 | 0.808
12 | LogRegCV(cv=5, max_iter=1000) | TF-IDF default, Improved Tokenizer, merge keywords-tokens | x | 0.813
13 | LogReg(max_iter=10000)| TF-IDF default, merge keywords-tokens, hyperparams tuning: C=1.206792| x | 0.801
14 | LogReg(max_iter=10000)| TF-IDF default, merge keywords-tokens, hyperparams tuning: C=1.7575 | x | 0.8091
15 | LogReg(max_iter=10000)| TF-IDF default, hyperparams tuning: C=1.7575 | x | 0.8126
16 | LogReg(max_iter=10000)| TF-IDF default, hyperparams tuning: C=1.7575 | x | 0.8126
17 | LogReg(max_iter=10000)| TF-IDF params tunning (ngram_range=(1, 3), min_df= 1, max_df=1.0)), C=1.206 | 0.807 | 0.8091
18 | LogReg(max_iter=10000)| TF-IDF params tunning (ngram_range=(1, 3), min_df= 1, max_df=4.0)), C=1.206, merge keywords-tokens | x | 0.8038
19 | KNN | K = 5 |  | 0.8038

## 📽️ Video

Here is the link to our video explaning the different steps we took for our project. Feel free to reach out if you would like any details.


 

