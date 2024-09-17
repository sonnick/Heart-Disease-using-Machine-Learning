# Heart-Disease-using-Machine-Learning
## Predicting Heart Disease using Machine Learning
### 1. Problem Defination

In our case, the problem we will be exploring is binary classification (a sample can only be one of two things).

This is because we're going to be using a number of differnet features (pieces of information) about a person to predict whether they have heart disease or not.

In a statement,

Given clinical parameters about a patient, can we predict whether or not they have heart disease?

### 2. Data
The original data came from the Cleveland database from UCI Machine Learning Repository.
Howevever, we've downloaded it in a formatted way from Kaggle.
The original database contains 76 attributes, but here only 14 attributes will be used. Attributes (also called features) are the variables what we'll use to predict our target variable.
We use the independent variables to predict our dependent variable.
Or in our case, the independent variables are a patients different medical attributes and the dependent variable is whether or not they have heart disease.

### 3. Evaluation
The evaluation metric for this machine learning project will be like
**If we can reach 95% accuracy at predicting whether or not a patient has heart disease during the proof of concept, we'll pursure this project.**
The reason this is helpful is it provides a rough goal for a machine learning engineer or data scientist to work towards.
However, due to the nature of experimentation, this requires a lot of effort and experimentation and also the evaluation metric may change over time. Thus we might end up achieving close to that if not the 95%

### 4. Features
Features are different parts of the data. During this step, we will to start find out what you can about the data.
One of the most common ways to do this, is to create a data dictionary.
Heart Disease Data Dictionary

### 5. Data Exploration (exploratory data analysis or EDA)
Once we've imported a dataset, the next step is to explore. There's no any formula of doing this. But our goal is to have a better understanding of our data variables and  more familiar with the dataset.

Compare different columns to each other, compare them to the target variable. Refer back to your data dictionary and remind yourself of what different columns mean.
Since EDA has no real set methodolgy, the following is a short check list you might want to walk through:

What question(s) are you trying to solve (or prove wrong)?
What kind of data do you have and how do you treat different types?
What’s missing from the data and how do you deal with it?
Where are the outliers and why should you care about them?
How can you add, change or remove features to get more out of your data?

### 6. Modeling
Once we've explored the data, now we'll try to use machine learning to predict our target variable based on the 13 independent variables.
And Remember our problem? which was **Given clinical parameters about a patient, can we predict whether or not they have heart disease?** That's what we'll be trying to answer.
And remember our evaluation metric?
If we can reach 95% accuracy at predicting whether or not a patient has heart disease during the proof of concept, we'll pursure this project

### Hyperparameter Tuning

### Evaluating a classification model, beyond accuracy
Now after we have tuned a model, we will getsome of the metrics we discussed before.
We want:
ROC curve and AUC score - `_RocCurveDisplay()_`
Note: This was previously sklearn.metrics.plot_roc_curve(), as of Scikit-Learn version 1.2+, it is sklearn.metrics.RocCurveDisplay().
Confusion matrix - `confusion_matrix()`
Classification report - `classification_report()`
Precision - `precision_score()`
Recall - `recall_score()`
F1-score - `f1_score()`

### Feature importance
Feature importance will be solving the question, "which features contributing most to the outcomes of the model?"
Or for our problem, trying to predict heart disease using a patient's medical characterisitcs, which charateristics contribute most to a model predicting whether someone has heart disease or not?
How each model finds patterns in data is slightly different, how a model judges how important those patterns are is different as well. This means for each model, there's a slightly different way of finding which features were most important.
