# HASOC-2020

This repository contains our (HRS-TECHIE) submissions to the HASOC 2020 competetion which is "Hate Speech and Offensive Content Identification in Indo-European Languages" at FIRE 2020.

# About HASOC 2020 -FIRE2020
The large fraction of hate speech and other offensive and objectionable content online poses a huge challenge to societies. Offensive language such as insulting, hurtful, derogatory or obscene content directed from one person to another person and open for others undermines objective discussions. Such type of language can be more increasingly found on the web and can lead to the radicalization of debates. Objectionable content can pose a threat to democracy. At the same time, open societies need to find an adequate way to react to such content without imposing rigid censorship regimes. As a consequence, many platforms of social media websites monitor user posts. This leads to a pressing demand for methods to automatically identify suspicious posts. Online communities, social media enterprises and technology companies have been investing heavily in technology and processes to identify offensive language in order to prevent abusive behavior in social media.

HASOC provides a forum and a data challenge for multilingual research on the identification of problematic content. This year, we offer again 2 sub-tasks for each language such as English, German and Hindi, alltogether over 10.000 annotated tweets from Twitter. Participants in this year’s shared task can choose to participate in one or two of the subtasks.

# Tasks

There are two sub-tasks in each of the languages. Below is a brief description of each task.

  # Sub-task A: Identifying Hate, offensive and profane content
   This task focus on Hate speech and Offensive language identification offered for English, German, and Hindi. Sub-task A is coarse-grained binary classification in which participating system are required to classify tweets into two classes, namely: Hate and Offensive (HOF) and Non- Hate and offensive (NOT).
   ### 1. NOT : 
    Non Hate-Offensive - This post does not contain any Hate speech, profane, offensive content.
   ### 2. HOF : 
    Hate and Offensive - This post contains Hate, offensive, and profane content.
   
 # Sub-task B: Discrimination between Hate, profane and offensive posts
  This sub-task is a fine-grained classification offered for English, German, and Hindi. Hate-speech and offensive posts from the sub-task A are further classified into three categories:
  ### HATE :
    Hate speech:- Posts under this class contain Hate speech content.
  ### OFFN :
    Offenive:- Posts under this class contain offensive content.
  ### PRFN :
    Profane:- These posts contain profane words.

  
# Our Submissions
We develped the Machine learning , Deep learning and Ensemble methodology ( Max voting ) based classifiers for the English data for Sub-task A and B.

This repo contains four IPython Notebooks which are containing the code for develop the classifiers to the challenge. 
 #### 1. ML_Ensemble for task-A.ipynb
 #### 2. DL_LSTM for task-A.ipynb
 #### 3. ML_Ensemble for task-B.ipynb
 #### 4. DL_Bi-GRU for task-B.ipynb
 

# 1. ML_Ensemble for task-A.ipynb
This notebook contains the code for reading the dataset,preprocessing of comments , creating TF_IDF vectors , creating Machine learning models (Naive Bayes , SVM , Decision tree, Random Forest )/ Ensemble model ( Max voting of 4 ML classifiers), training and predicting the labels of the test data for sub-task A.

# 2. DL_LSTM for task-A.ipynb
This notebook contains the code for reading the dataset,preprocessing of comments , Download Glove word embedding and generate embedding matrix for data, creating LSTM model, training and predicting the labels of the test data for sub-task A.

# 3. ML_Ensemble for task-B.ipynb
This notebook contains the code for reading the dataset,preprocessing of comments , creating TF_IDF vectors , creating Machine learning models (Naive Bayes , SVM , Decision tree, Random Forest )/ Ensemble model ( Max voting of 4 ML classifiers), training and predicting the labels of the test data for sub-task B.

# 4. DL_Bi-GRU for task-B.ipynb
This notebook contains the code for reading the dataset,preprocessing of comments , Download Glove word embedding and generate embedding matrix for data, creating Bi-GRU model, training and predicting the labels of the test data for sub-task A.

# Results
   ##### LSTM classifier 
achieves the highest macro average F1-score 
##### 0.5002  
compare than our other classifiers and got 
##### 12th place
in the 
##### Sub-task A leaderboard .
   ##### Ensemble classifier achieves the highest macro average F1-score 0.2426  compare than our other classifiers and got 9th place in the Sub-task B leaderboard .
