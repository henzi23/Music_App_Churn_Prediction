# Music App Churn Prediction
#### Udacity Data Science Capstone project
#### Prepared by James Henzi

## Project Overview
Have you ever noticed that it seems like apps know you’re considering canceling membership? They always come with some type of offer or incentive (reduced fees, etc) at just the right moment. This is hardly a coincidence.  Application are constantly collect data regarding user activity.  The companies making the apps use this "big data" lake to analyze and predict user behaviors.  Being able to translate this data into the correct actions can make or break a company.

For this project we will look at a dataset from a fictitious music app called Sparkify (thanks to Udacity for providing this dataset).  The the goal of the project is to predict use the data to predict user churn.  This notebook will set through the process of loading the dataset, exploring the data, creating a feature engineered set include features of interest, building a machine learning model, and evaluating this model.

Throughout the project big data tools will be utilized.  Specifically we will leverage Spark and the associated relevant libraries (pyspark and pyspark.ml).

## Problem Statement
As mentioned in the Overview we will be using data for a fictitious music app called Sparkify. For an application of this type retaining users is a huge priority as users translate into money (subscription fees, advertisement revenue).  As such it is critical for these companies to known when a user might churn (leave/quit the app).  If a company can predict when users might be thinking about leaving they can take countermeasures to try to keep that user or group of users (provide incentives, perhaps add features, etc).  
For this project we will use a modest set of data covering actions of a small sample of users for a few monthes time.  Based on the actions taken by these users we will try to build a model to predict which users will churn.  The steps we will take are:
* Load and Clean Data: read in the json datatset, evaluate the cleanliness and completeness, and clean as needed
* Exploratory Data Analysis: define churn and create a churn attribute.  Then test hypotheses about user behavior (churn vs no churn).  Based on our findings we will determine features of interest.
* Feature Engineering: build an ETL pipeline to take input data like our sample and transpose them into a summarized datatset including our desired features of interest
* Build Machine Learning Models: build baseline models with a number of classification method, choose the best model, feature optimize the model, and finally test the results of the optimized model.


## Results
We were successful in gaining some insight into how apps use their data to predict user behavior. With a relatively modest sample set from the fictitious music app we successfully:
* Identifying features of interest: utilizing the user action data (similar to data any app would collect) we used hypotheses regarding expected user behavior to determine features of interest.
* Build a ETL pipeline to take the raw data and feature engineer it into an aggregated set including our desired features of interest.
* Training a model: we utilized the determined features of interest to train multiple baseline models and utilized the F1 metric to compare models. We then chose the best model to move forward and tune.
* Evaluate our model: we then evaluated our model and found it to yield 80% accurate predictions on a test dataset.

Detailed discussion of the analysis results can be found in an article at:https://medium.com/@jameshenzi/how-do-apps-know-were-thinking-of-canceling-3f50bc5b4af3

## Getting Started

This repo includes 4 main files:
* Sparkify.ipynb : Jupyter notebook detailing the data review, exploratory data analysis, feature engineering, and model development.
* Sparkify.html : html version of the Jupyter notebook
* mini_sparkify_event_data.zip : compressed file with json sample data file used by Jupyter notebook
* plots folder: folder with .jpg versions of plots

### Prerequisites

All programming utilizes Python 3.  All coding is in a Jupyter notebook.  Key packages utilized are pyspark, datetime, numpy, pandas, and matplotlib

### Installation/Deployment

To run the project files copy Jupyter notebook and data zip file to a single directory on your local machine.  Extract the json file from the .zip.  Be sure not to change the file name.  From local command Anaconda environment open and run the Jupyter notebook.

## Author

* James Henzi


## Acknowledgments

* Udacity - for project inspiration and guidance
