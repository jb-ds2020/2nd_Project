# Predictive modeling credit default - Lending Club
This is our second project of the Data Science bootcamp at neuefische. We **(Jonas Bechthold & Silas Mederer)** were asked to develop a **model to predict the default credits** based on a training set prohibited by Lending Club on [kaggel.com.](http://www.kaggle.com "kaggel.com.") The dataset holds 42.536 entries, 51 possible features and the label ‘loan_status’ from (Q4-2007 to Q1-2012). The purpose of the analysis is to reduce defaults. **We will use machine learning models to analyze credit risk as a binary classification problem.**
![picture by: Lending Club 2020](/presentation/2020-lending-club-head.png) 

picture by: Lending Club 2020

In this repository you can find our ideas and models with which we tried to solve the given task.

- [Here you can find our exploratory data analysis (EDA)](http://https://github.com/jb-ds2020/2nd_Project/blob/main/2020-LendingClub_EDA.ipynb "Here you can find our exploratory data analysis (EDA)") and also oriented on the data science lifecycle, a chapter of business understanding, data mining and cleaning. This notebook is important to know the data and all steps are commented as well, so that you will get an impression by skimming it.

- After the cleansing and EDA we choose three machine learning approaches [Decision Trees](http://https://github.com/jb-ds2020/2nd_Project/blob/main/2020-LendingClub_DecisionTrees.ipynb "Decision Trees"), [Classification](http://https://github.com/jb-ds2020/2nd_Project/blob/main/2020-LendingClub_Classicationmethods.ipynb "Classification") and [Ensemble Methods](http://https://github.com/jb-ds2020/2nd_Project/blob/main/2020-LendingClub_EnsembleMethods.ipynb "Ensemble Methods")) . You can find one notebook for each of them.

- At least we tried to build a [regression (OLS)](http://https://github.com/jb-ds2020/2nd_Project/blob/main/2020-LandingClub-OLS-int_rate.ipynb "regression (OLS)") to predict the ‘int_rate’ of the credits. It seems to be very important to choose other features to explain this label. In our model we had an R2 below 15%. Since everything was technically correct, it must be the features. :)

- At least you can find a presentation held on 08th October in front of non technical but data interested people.

## Problem definition in one sentence:
**Predict the default credits and avoid false positives**
## Problem definition given by Lending Club on [kaggle.com](http://www.kaggle.com "kaggle.com") and [neuefische DS Bootcamp](http://https://www.neuefische.de/weiterbildung/data-science "neuefische DS Bootcamp"):
How to choose the performance metrics? - well the model (whichever you pick) will be used to determine who should be approved for a loan and who shouldn’t, denying the loan to a client who will end up paying in full (false positives) represents a loss, but because interest is usually only a portion of principal the company will most likely be more comfortable not taking the chance when the risk is not to get reimbursed at all and lose the entire principal which represents a higher amount. Thus the main concern here is to avoid approving somebody who won't be able to repay or in other words avoid false negatives. This is achieved by a model with a high recall rate. What would be the right performance metric - precision, recall, accuracy, F1 score, or something else?

## Future work
- **Other perspective other needs:** We focussed on the investors perspective with a high recall so that they get their money back. But what about the club? Then we need another metric (F1 score) to fit the models. Or we ask from the borrower perspective “What would be my ‘grade’ or ‘int_rate’?”. In this case we need to train a regression model, choose other features and metrics.
- **Improve the models:** Higher precision to reduce False- Negatives, these people paid back but were wrong predicted. It’s a loss for all stakeholders.

------------

**We had great fun working together on this project and are curious to hear what you have to say. Please do not hesitate to contact us if you have any questions. Hope you enjoy it too.**
