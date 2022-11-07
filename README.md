# MechaCar_Statistical_Analysis


 ## Linear Regression to Predict MPG
 
* Vechicle length and ground clearance provided a non-random amount of variance to the mpg values in the dataset due to there P values being lower than .05?
 
* Is the slope of the linear model is much smaller than the assumed significance level of 0.05% which indicates that the slope of this linear model is not zero.

* This model is not effectivve at predicting mpg as it has a squared value of .7149

<img src="Resources/Images/pvalue_rsquared.png" align="center">

## Summary Statistics on Suspension Coils

* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

When we look at the total summary, the variance of the coils is 62.29 Pounds per Square inch, which is within the 100 PSI variance requirement.

<img src="Resources/Images/TotalSummary.png" align="center">

When looking at the individual lots, Lots 1 and 2 are well within the 100 PSI variance requirement with variances of 0.98 and 7.47. However, when looking at Lot 3 we see a variance of 170.29, which greatly exceeds the limit. 

In summary it meets the demand manufacturing when looking at all lots in total but not when looking at the lots individually.

<img src="Resources/Images/LotSummary.png" align="center">

## T-Tests on Suspension Coils
When looking at tge total we see the sample mean is 1498.78.  With a p-Value of 0.06, which is greater than the common significance level of 0.05,  This indicates that there is not enough evidence to support rejecting the null hypothesis.

#### All Lots
<img src="Resources/Images/t-test_All_Lots.png" align="center">  

Looking at the indiviual lots we see that Lot 1 has a sample mean of 1500 with a p-Value of 1.  Meaning we cannot reject.  Lot 2 has a sample mean of 1500.02, and a p-Value of 0.61.  Meaning we cannot reject. 

Looking at Lot 3 we see it has a sample mean of 1496.14 and a p-Value is 0.04, which is lower than the common significance level of 0.05 which leads us to reject the null hypothesis that the presumed population mean are not statistically different.

#### Lot 1
<img src="Resources/Images/t-test-Lot-1.png" align="center">  

#### Lot 2
<img src="Resources/Images/t-test-Lot-2.png" align="center">  

#### Lot 3
<img src="Resources/Images/t-test-Lot-3.png" align="center">  



## Study Design: MechaCar vs Competition

Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

In my statistical study I would perform multiple linear regression analysis to identify which variables in the metrics provided below drive the needle in determining best in class.

The ultimate goal is to determine if MechaCar will be the best in class. 

I will examine the following independent variables

* Safety Rating
* Resale Value
* Fuel Efficiency (MPG)
* Owner Satisfaction Survey Scores
* Technology Package Satisfaction Survey Scores

I would use the sales price as the dependent variable.

### Hypothesis: 

Null Hypothesis: MechaCar is best in class based on its performance of key metrics

Alternative Hypothesis: MechaCar is not best in class based on performance of key metrics

A multiple linear regression would be used to determine which factors have the highest correlation with the selling price.

