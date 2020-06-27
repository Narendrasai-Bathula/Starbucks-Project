# Starbucks Capstone Challenge
Project in Data Scientist Nanodegree of Udacity

![Intro Pic](intro.jpeg)

## Project Motivation<a name="motivation"></a>

It is the Starbuck's Capstone Challenge of the Data Scientist Nanodegree in Udacity. We get the dataset from the program that creates the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers. We want to make a recommendation engine that recommends Starbucks which offer should be sent to a particular customer.

## Installation<a name="Installation"></a>
The project was written in python uaing jupyter notebook

Libraries used in this are
pandas

numpy

math

json

sklearn.model_selection (train_test_split module)

sklearn.preprocessing (StandardScaler, PolynomialFeatures)

from sklearn.tree (DecisionTreeClassifier,DecisionTreeRegressor)

sklearn.ensemble (RandomForestClassifier)

sklearn.metrics (mean_squared_error,classification_report)

sklearn.linear_model (Ridge)

time

sklearn.model_selection (GridSearchCV)

matplotlib

## File Descriptions <a name="files"></a>
The notebook available here showcases work related to the above questions.  

This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products. and store in zip file

The data is contained in three files:
- `portfolio.json` - containing offer ids and meta data about each offer (duration, type, etc.)
- `profile.json` - demographic data for each customer
- `transcript.json` - records for transactions, offers received, offers viewed, and offers completed

## Author <a name="Author"></a>
The Github Repository of author is [here](https://github.com/Narendrasai-Bathula/Starbucks-Project)

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@nani90103/starbucks-project-d9de78c3bfd6).

Based on the transcript records, we build an user-item-matrix that represents how users responded to the offers they received. We then split the records into the training set and the test set and trained our SVD algorithm to predict how a user responses to a particular offer. We achieved the lowest mean square error around 0.003823 with 15 latent features with the training set and around 0.009175 with 10 latent features with the testing set. After that, we created a recommendation engine that recommends Starbucks which offer should be sent to a particular user

we found out which demographic groups respond best to which offer type. Female respond much better than men, in both BOGO and discount. Men react slightly better to discount than BOGO. We also found that it is better to promote the offer via social media. Among the ten offers, sending buy 10 dollars get 2 dollars off within 10 days offer via email, web, mobile and social makes Starbucks gain more. It is the best offer so far!
###LICENSES AND ACKNOWLEDGEMENTS
The data given by udacity by datascience nanodegree program
