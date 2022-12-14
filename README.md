<!-- PROJECT LOGO -->
<br />
<p align="center">
  
  <a href="https://github.com/OmoyeniO/Churn-Prediction-Using-Spark">
    <img src="sparkify_img.png" alt="Logo", width = 500 >
  </a>
  
</p>







### Table of Contents

1. [Background](#Background)
2. [Installation](#Installation)
3. [Project Motivation](#Motivation)
4. [Files Description](#Files)
5. [Results](#Results)
6. [Acknowledgements](#Acknowledgements)



# Churn Prediction Using Spark



##  Background<a name="Background"></a>
Sparkify is a music streaming service invented by Udacity. With Sparkify users can listen to music for free (with ads between songs) or subscribe to the platform at a flat rate. Users can upgrade, downgrade, or cancel their subscriptions as well.

The task is to predict the users who are going to leave in order to offer them a great discount before they cancel their subscription and leave the platform.

Project Steps:

* Exploratory Data Analysis (EDA)
* Feature engineering
* Model building 
* Evaluation
* Results
* Conclusion




##  Installation<a name="Installation"></a>

Required Python libraries:

* PySpark 
* Pandas
* Matplotlib 
* Seaborn  





## Project Motivation<a name="Motivation"></a>

This is a Capstone project done in conjuction with Udacity as part of the requirement for the Data Science Nanodegree program.

The goal of this project is to learn how to manipulate large and realistic datasets with Spark to engineer relevant features for predicting churn. I want to learn how to use Spark MLlib to build machine learning models with large datasets, far beyond what could be done with non-distributed technologies like scikit-learn.





## Files Description<a name="files"></a>

1. `mini_sparkify_event_data.json` is the data used and it is a mini subset (128MB) of the full dataset available (12GB)
2. [Sparkify.ipynb](./Sparkify.ipynb) notebook contains all steps involved in the project
3. [gbt.model](./gbt.model) The GBT model built
4. [svm.model](./svm.model)The SVM model 
5. [logistic.model](./logistic.model)The Logistic model 





## Results<a name="results"></a> 

After carrying out EDA on the data understanding the different levels of the dataset and how it impacted churn. We created features that were later used in building three machine learning models, namely: Logistic regression, Support Vector Machine(SVM), and Graident Boosted Tree (GBT).

Amongst the three models, the GBT performed best with good f1 scores and hight accuracy score of 99% although it took a longer time to train.

The models resulted in:

* logistic regression (best f1 score 0.7641) (Accuracy of the best Logistic model: 83.88%)
* Support Vector Machine (best f1 score 0.7534) (Accuracy of the best SVM model: 83.69%)
* Gradient Boosted Tree (best f1 score 0.7621 ) (Accuracy of the best GBT model: 99.05%)

The best being the GBT




## Blog

More detailed findings and analysis can be found in the blog post on [Medium](https://omoyeni-ogundipe.medium.com/churn-prediction-using-pyspark-on-big-data-fce0e0f0f1d4) 





## Acknowledgements<a name="Acknowledgements"></a> 
The data used in this project was provided by Udacity as part of the ***[Data Science Nanodegree Program](https://www.udacity.com/course/data-scientist-nanodegree--nd025)*** 




