# Music App Churn Prediction

Project to predict user churn (account cancellation) for a fictional music app (Sparkify).  This project takes user action records (user info, page visited, timestamp, etc) as inputs.  Exploratory data analysis is perfroemd on these records focusing on evaluating hypotheses regarding churn user behaviors.  Based on the findings from the EDA features of interest are engineered.  The resulting features are used to generate a ML model for prediction.  For all of this effort Spark is utilized to facilitate the data processing requirements.

## Getting Started

This repo includes 3 main files:
* Sparkify.ipynb : Jupyter notebook detailing the data review, exploratory data analysis, feature engineering, and model development.
* Sparkify.html : html version of the Jupyter notebook
* mini_sparkify_event_data.zip : compressed file with json sample data file used by Jupyter notebook

### Prerequisites

All programming utilizes Python 3.  All coding is in a Jupyter notebook.  Key packages utilized are pyspark, datetime, numpy, pandas, and matplotlib

### Installation/Deployment

To run the project files copy Jupyter notebook and data zip file to a single directory on your local machine.  Extract the json file from the .zip.  Be sure not to change the file name.  From local command Anaconda environment open and run the Jupyter notebook.

## Author

* James Henzi


## Acknowledgments

* Udacity - for project inspiration and guidance
