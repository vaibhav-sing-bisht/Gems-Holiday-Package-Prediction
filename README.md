## Gems-Holiday-Package-Prediction
This project is based on 2 cases studies : Gems Price Prediction and Holiday Package prediction.

In the first case study, concepts of linear regression are tested and it is expected from the learner to predict the price of gems based on multiple variables to help company maximize profits. 

In the second case, concepts of logistic regression and linear discriminant analysis are tested. One has to predict if the customer will purchase the holiday package to target the relevant customer base.  Skills and Tools  Linear Regression, Logistic Regression, Linear discriminant Analysis

## Skills and Tools

Linear Regression, Logistic Regression, Linear discriminant Analysis

![shutterstock-181978181](https://user-images.githubusercontent.com/87828805/147233447-8fd523fe-1765-4859-8c48-3636c21fb341.jpg)

## Problem 1: Linear Regression


You are hired by a company Gem Stones co ltd, which is a cubic zirconia manufacturer. You are provided with the dataset containing the prices and other attributes of almost 27,000 cubic zirconia (which is an inexpensive diamond alternative with many of the same qualities as a diamond). The company is earning different profits on different prize slots. You have to help the company in predicting the price for the stone on the bases of the details given in the dataset so it can distinguish between higher profitable stones and lower profitable stones so as to have better profit share. Also, provide them with the best 5 attributes that are most important.


### Data Dictionary:

### Variable Name	Description
Carat	 Carat weight of the cubic zirconia.

Cut	 Describe the cut quality of the cubic zirconia. Quality is increasing order Fair, Good, Very Good, Premium, Ideal.

Color 	 Colour of the cubic zirconia.With D being the worst and J the best.

Clarity	Clarity refers to the absence of the Inclusions and Blemishes. (In order from Worst to Best in terms of avg price) IF, VVS1, VVS2, VS1, VS2, Sl1, Sl2, l1

Depth	 The Height of cubic zirconia, measured from the Culet to the table, divided by its average Girdle Diameter.

Table	 The Width of the cubic zirconia's Table expressed as a Percentage of its Average Diameter.

Price	 the Price of the cubic zirconia.

X	 Length of the cubic zirconia in mm.

Y	 Width of the cubic zirconia in mm.

Z	 Height of the cubic zirconia in mm.

## Problem 2: Logistic Regression and LDA


You are hired by a tour and travel agency which deals in selling holiday packages. You are provided details of 872 employees of a company. Among these employees, some opted for the package and some didn't. You have to help the company in predicting whether an employee will opt for the package or not on the basis of the information given in the data set. Also, find out the important factors on the basis of which the company will focus on particular employees to sell their packages.

### Dataset for Problem 2: Holiday_Package.csv

### Data Dictionary:

### Variable Name	Description
Holiday_Package 	 Opted for Holiday Package yes/no?

Salary 	 Employee salary

age 	 Age in years

edu 	 Years of formal education

no_young_children 	 The number of young children (younger than 7 years)

no_older_children 	 Number of older children

foreign 	 foreigner Yes/No

From the above table we can easily find out the values of Accuracy, AUC, Recall, Precision, and F-1 Score of two different model which Logistic Regression and LDA.
Inference From the above table:-
From the above table we can easily find out the values of Accuracy, AUC, Recall, Precision, and F-1 Score of two different model which Logistic Regression and LDA.
Inference From the above table:-
1) Accuracy is almost same for all except LR test data which is 0.65
2) AUC for LR train and LDA train has same area under the curve about 0.73 .Whereas LDA test has least AUC of abut 0.70
3) Recall for LDA test is the highest of about 0.73 and least is for LR test of about 0.51
4) Precision in LDA test is lacking of about 0.61 while rest are having a value of 065
5) F1 Score for the LDA test is the highest of about 0.66 whereas LR Test performed poorly of about 0.57

Since we are building a model to predict if a person has opted holiday package or not, for practical purposes, we will be more interested in correctly classifying 1 (having opted claim) than 0(not opted).


LDA test model is predicting 73 percent that how many of the actual True data points are identified as True data points by the model which is highest in all other model.
The F1 score which is  weighted average of Precision and Recall is 66% again shown  by LDA test model which is the highest score which takes both false positives and false negatives into account.

### So LDA is the best model for the company in predicting whether an employee will opt for the package or not.
