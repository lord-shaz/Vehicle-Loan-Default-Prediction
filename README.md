# LTFS-Data-Science-FinHack.
----
The objective of this project is to predict the probability of borrower defaulting on a vehicle loan in the first EMI (Equated Monthly Installments) on the due date.

## Overview:
----
**End-user:** Financial institution

**Objective:** The objective of this project is to predict the probability of loanee or borrower defaulting on a vehicle loan in the first EMI (Equated Monthly Instalments) on the due date.   
**Dataset:** The Vehicle Loan Default Prediction dataset includes following features:
**Dependent feature:** loan_default
**Independent features:** disbursed_amount, asset_cost, ltv, PERFORM_CNS.SCORE etc.
The dataset contains **345550** rows and **41** features.

## Data Cleaning:
-----
* Combining training and testing data.
* Checking missing values in data. 
* Imputing Employment.Type missing values with 'Self employed' values.
* Checking the outliers using boxplot.
* Removing the outliers of 'disbursed_amount' & 'asset_cost' features.

## Feature Enginnering & Feature Selection:
-----
* Calculating Age column using 'Date.of.Birth'.
* Calculating 'AVERAGE.ACCT.AGE' and 'CREDIT.HISTORY.LENGTH' in months.
* Creating bins of PERFORM_CNS.SCORE and LTV.
* Replacing Values of PERFORM_CNS.SCORE.DESCRIPTION.
* Generating New Features like 'ACTIVE.ACCTS','CURRENT.BALANCE' etc.
* Dropping irrelevant columns like 'DisbursalDate', 'Current_pincode_ID' ,'NO.OF_INQUIRIES' etc.

## Model Creation:
-----
CatBoost Classifier: ROC AUC Score: **0.6442**

## AUC ROC:
-----
![AUC_ROC](https://github.com/ShehzadaAlam/LTFS-Data-Science-FinHack/blob/master/AUC_ROC_Curve.png "AUC_ROC")

----
<p>Thank You!	
<p><!-- Place this tag where you want the button to render. -->
<a class="github-button" href="https://github.com/ShehzadaAlam" aria-label="Follow @ShehzadaAlam on GitHub">Follow @ShehzadaAlam</a>



