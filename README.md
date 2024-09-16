<!--# Hate-Speech-Event-Detection-CASE-EACL-2024 -->
# Shared task on Hate Speech and Stance Detection during Climate Activism [CASE 2024 at EACL 2024]

We have participated in the shared task on **Climate Activism Stance and Hate Event Detection Shared Task at CASE@EACL2024** in the CASE 2024 Competition and obtained remarkable positions 1st, 5th and 13th [Check Standings](https://codalab.lisn.upsaclay.fr/competitions/16206#results) in the 3 subtasks of this task. Here is the [System Description Paper of our Model](https://aclanthology.org/2024.case-1.20/). The full task description is given below:

Hate speech detection and stance detection are some of the most important aspects of event identification during climate change activism events. In the case of hate speech detection, the event is the occurrence of hate speech, the entity is the target of the hate speech, and the relationship is the connection between the two. The hate speech event has targets to which hate is directed. Identification of targets is an important task within hate speech event detection. Additionally, stance event detection is an important part of assessing the dynamics of protests and activisms for climate change. This helps to understand whether the activist movements and protests are being supported or opposed. This task will have three subtasks (i) Hate speech identification (ii) Targets of Hate Speech Identification (iii) Stance Detection.

### Sub-task A: Hate Speech Detection

The goal of this task is to identify whether the given text contains hate speech or not. The text, which are the dataset for this subtask, will have annotations for the prevalence of hate speech.

### Sub-task B: Target Detection

The goal of this subtask is to identify the targets of hate speech in a given hateful text. The text are annotated for "individual", "organization", and "community" targets.

### Sub-task C: Stance Detection

The goal of this subtask is to identify the stance in a given text. The text are annotated for "support", "oppose", and "neutral" stance.

## What we have accomplished in this task
The escalating impact of climate change on our environment and lives has spurred a global surge in climate change activism. However, the misuse of social media platforms like Twitter has opened the door to the spread of hatred against activism, targeting individuals, organizations, or entire communities. Also, the identification of the stance in a tweet holds paramount significance, especially in the context of understanding the success of activism. So, to address the challenge of detecting such hate tweets, identifying their targets, and classifying stances from tweets, this shared task introduced three sub-tasks, each aiming to address exactly one mentioned issue. We participated in all three sub-tasks and in this paper, we showed a comparative analysis between the different machine learning (ML), deep learning (DL), hybrid, and transformer models. Our approach involved proper hyper-parameter tuning of models and effectively **handling class imbalance datasets** through data oversampling. Notably, our fine-tuned m-BERT achieved a **macro-average _F1_score of 0.91 in sub-task A_ (Hate Speech Detection) and _0.74 in sub-task B_ (Target Identification)**. On the other hand, **Climate-BERT achieved a _F1-score of 0.67 in sub-task C_**. These scores positioned us at the forefront, securing **_1st, 6th, and 15th ranks_ in the respective sub-tasks**.

## Models We Have Experimented
### ML Models
+ **Random Forest with TF-IDF and Word2Vec** 
+ **Logistic Regression with TF-IDF and Word2Vec** 
+ **Support Vector Machine with TF-IDF and Word2Vec** 
+ **Multinomial Naive Bayes with TF-IDF and Word2Vec** 
### DL Models
+ **BiLSTM with Word2vec, Glove, and FastText**
+ **BiGRU with Word2vec, Glove, and FastText**
+ **BiLSTM+CNN with Word2vec, Glove, and FastText**
+ **CNN+BiGRU with Word2vec, Glove, and FastText**
### Transformers
+ **m-BERT**
+ **Distil-BERT**
+ **XLM-R**
+ **Climate-BERT**
### Hybrid Models
+ **m-BERT+BiLSTM**
+ **m-BERT+BiLSTM+CNN**
