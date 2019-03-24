# Music App Churn Prediction

Project to predict user churn (account cancellation) for a fictional music app (Sparkify).  This project takes user action records (user info, page visited, timestamp, etc) as inputs.  Exploratory data analysis is perfroemd on these records focusing on evaluating hypotheses regarding churn user behaviors.  Based on the findings from the EDA features of interest are engineered.  The resulting features are used to generate a ML model for prediction.  For all of this effort Spark is utilized to facilitate the data processing requirements.

Summary of results:
I was able to gain some insight into how apps use their data to predict user behavior. With a relatively modest sample set from the fictitious music app we were successful at:
* Identifying features of interest: utilizing the user action data (similar to data any app would collect) we used hypotheses regarding expected user behavior to determine features of interest.
* Training a model: we utilized the determined features of interest to train multiple baseline models and utilized the F1 metric to compare models. We then chose the best model to move forward and tune.
* Evaluate our model: we then evaluated our model and found it to yield 86.7% accurate predictions on a test dataset.

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
