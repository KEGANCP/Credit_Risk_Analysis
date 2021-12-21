# Credit_Risk_Analysis

<p align="center">
  <img src="https://github.com/KEGANCP/Credit_Risk_Analysis/blob/main/Resources/Banner.jpg" alt="HEADER"/>
</p>

----

### Project Overview
Utilizing a credit card credt dataset from LendingClub, I have used Python to build machine learning models to find methods to best predict credit risks.

#### Methods Utilized:
  - Oversampling via **RandomOverSampler** and **SMOTE**
  - Undersampling via **ClusterCentroids**
  - Combination of over & under sample via **SMOTEEN**
  - Compare **BalancedRandomClassifier** v **EasyEnsembleClassifier**

#### Tools Utilized
  - Data Source via LendingClub
  - Python
  - Jupyter Notebook

----

### Analysis Results
Review the below images of several different reports and their findings.
----
#### RandomOverSampler Model
<p align="center">
  <img src="https://github.com/KEGANCP/Credit_Risk_Analysis/blob/main/Resources/RandomOverSample.png" alt="oversampler"/>
</p>

Per the above;
- Balance accuracy is 65%
- High_risk precision is 1%, 72% recall, and F1 of 2%
- Low_risk precision is 100% with recall of 59%


#### SMOTE Model
<p align="center">
  <img src="https://github.com/KEGANCP/Credit_Risk_Analysis/blob/main/Resources/SMOTE.png" alt="SMOTE"/>
</p>

Per the above;
- Balance accuracy is 66%
- High_risk precision is 1%, 63% recall, and F1 of 2%
- Low_risk precision is 100% with recall of 69%

#### ClusterCentroids Model
<p align="center">
  <img src="https://github.com/KEGANCP/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids.png" alt="ClusterCent"/>
</p>

Per the above;
- Balance accuracy is 54%
- High_risk precision is 1%, 69% recall, and F1 of 1%
- Low_risk precision is 100% with recall of 40%

#### SMOTEENN Model
<p align="center">
  <img src="SMOTEEN" alt="SMOTEEN"/>
</p>


#### BalancedRandomForestClassifier Model
<p align="center">
  <img src="https://github.com/KEGANCP/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassfier.png" alt="BRFC"/>
</p>

Per the above;
- Balance accuracy is 79%
- High_risk precision is 4%, 67% recall, and F1 of 7%
- Low_risk precision is 100% with recall of 91%

#### EasyEnsembleClassifier Model
<p align="center">
  <img src="https://github.com/KEGANCP/Credit_Risk_Analysis/blob/main/Resources/EEC.png" alt="EEC"/>
</p>

Per the above;
- Balance accuracy is 92%
- High_risk precision is 7%, 90% recall, and F1 of 14%
- Low_risk precision is 100% with recall of 94%
---- 
### Analysis Summary
----
Of all the data presented above, the best option is the EasyEnsembleClassifier model which is our highest recall percentage at over 90% got our high risk credit. This is comfirming our best choice to correctly detect most of the "high risk credit" within our data set. 
There is still room for error using this model as the preceision percentage is low (although the highest amongst all of our current options), I would recommend further research to determine if there is a more accurate model to utilize. In efforts to elude any potential loss of revenue, there may be an oppurtunity to implement a secondary credit check by identifying key variables such as the requested loan amount compared to the requestors salary, for example.
