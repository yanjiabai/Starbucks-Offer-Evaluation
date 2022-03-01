# Starbucks-Offer-Evaluation
This is a capstone project to evaluate offers sent on Starbucks app for Udacity Data Scientist Nanodegree Program.

## Introduction
The data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app, showing what types of offers were sent to what types of customers and whether the offers were viewed and/or completed. In the jupyter notebook, I combined the information in the original data sets (stored in the data folder), did data visualizations to explore the data set, and finally analyzed what offers were more likely to be completed using machine learning models. 

## Summary of results
My goal is to train a classification model to classify what types of customers and offers lead to an offer being completed. I tried random forest classifier and linear support vector classification with grid search and cross validation. Both give high scores (>0.75 in accuracy score and f1 score), but the former has a much shorter training time. I therefore suggest using random forest classifier. The trained model is stored in rfc.pkl.

## Files
* data
  ** portfolio.json | data about the offers sent
  ** profile.json | data about customers
  ** transcript.json | transaction data about customers receiving, viewing, and completing offers
* README.md
* Starbucks_Capstone_notebook.ipynb | the jupyter notebook containing my codes and comments
* rfc.pkl | pickle file storing the trained model using Random Forest Classifier
* svm.pkl | pickle file storing the trained model using (linear) SVM

## Libraries used and environment
This project used the following libraries:
* pandas
* numpy
* math
* time
* json
* sqlite3
* sqlalchemy
* pickle
* matplotlib
* sklearn

The jupyter notebook should run without problem under Python 3.6.3.

## Blog article
I wrote a blog article to summarize the main findings. The link is here: https://joyybai.medium.com/what-offers-attract-starbucks-customers-the-most-782689dcd260.
