# Title
Important News Detection

# Abstract
News Classification is a fundamental task in Text
Mining and Natural Language Processing(NLP). According to
large amount of data in this area, people needs to save their
times and first check the important News so we need to do this
task automatically. Machine Learning models tries to do tasks
automatically and time efficient by acceptable accuracy in many
fields and in this work we use different models for find important
News in different categorise

# Models' Description

In thisproject we use machine learning for intelligent and aoutomated important news detection on our dataset that consist of 4000 sample Persian News from different categorise and different journals for first time in this eara. We achived worthy results that best of them are realesd in results section.
All models used in this project:
* Classic machine learning models:
  * Logistic Regression
  * SVM
  * Naive Bayes
  * Decision Tree
  * Random Forest

* Deep learning models:
  * BiLSTM Attention Based 
  * Bert
  * Roberta
  
  
# Files' Description

* **analysis/**
  * **Kappa.ipynb:** This file caontains computation of kappa and fleiss kappa agreement on data and each category
  * **scorings.ipynb:** This file contains some experiments on models like computing correlation of news category and important news, computation of error distribution of wrong predicted data and computation of ensemble score of logistic regression, bilstm and roberta models
* **best_model_wrapper/** 
  * **Roberta_News_FInal_Category_Wrapper.ipynb:** this file contains a wrapper for our best single model that you can run tests on
* **classic_models/**
  * **Classical_ML.ipynb:** This file contain implementation of Logistic Regresseion, SVM, Naive Bayes, Decision Tree and Random Forest models that traint and evaluate by k-fold cross validation teqnique and after hyper parameter tunung results on test dataset are realesd.
* **lstm_models/**
  * **BiLSTM_attention_last.ipynb:** This file contain implementation of BiLSTM Attention Based model that implement by keras frame work. This model evaluate by validation data and hyperparameter tuning on them and final results on test dataset are realeased.
* **transformer_models/**
  * **Bert_News_Final.ipynb:** This file conatain implemetation of partbert and training, evaluation and testing on data
  * **Roberta_News_FInal.ipynb:** This file conatain implemetation of parsroberta and training, evaluation and testing on data
  * **Roberta_News_FInal_Category.ipynb:** This file conatain implemetation of parsroberta with category as an extra input to model and training, evaluation and testing on data
  * **Roberta_News_FInal_Keywords.ipynb:** This file conatain implemetation of parsroberta with keywords as an extra input to model and training, evaluation and testing on data
  * **Roberta_News_Final_Oversampling.ipynb:** This file conatain implemetation of parsroberta with oversampling of imporatant data and training, evaluation and testing on data
  * **Roberta_News_KMeans.ipynb:** This file conatain implemetation of parsroberta with kmeans sampling of non-imporatant data and training, evaluation and testing on data
  * **Roberta_News_Agency_Bias.ipynb:** This file conatain implemetation of parsroberta with source-names removed from input text to model and training, evaluation and testing on data
  
# Results

| Model Name | F1-Macro |
| :-------------: | :-------------: |
| Naive Bayes  | 50.3 %  |
| Random Forest  | 55.3 %  |
| Drecision Tree  | 56.8 %  |
| Logistic Regression  | 64.9 %  |
| Support Vector Machine  | 64.9 %  |
| Bilstm  | 62.4 %  |
| Bert  | 62.4 %  |
| Roberta + KMeans Sampling  | 60.0 %  |
| Roberta + Oversampling  | 64.8 %  |
| Roberta + Keywords  | 62.6 %  |
| Roberta + Category  | **66.8 %**  |
| Logistic Regression + Bilstm + Roberta  | **67.5 %**  |

# intractive web base 

![Capture11](https://user-images.githubusercontent.com/50262458/154755508-6bea3b74-e88f-45f3-95aa-fccead937c7c.PNG)


