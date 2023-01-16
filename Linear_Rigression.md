# Linear Regression
## What is Linear Regression ?

Linear regression fits a straight line or surface that minimizes the discrepancies between predicted and actual output values. There are simple linear regression calculators that use a “least squares” method to discover the best-fit line for a set of paired data.

## Idea


<img src="Linear Regression/img/idea_1.png" height="300" width="400">  | <img src="Linear Regression/img/idea_14.png" height="300" width="400">
------------- | -------------
<img src="Linear Regression/img/idea_15.png" height="300" width="400">  | <img src="Linear Regression/img/idea_18.png" height="300" width="400">
<img src="Linear Regression/img/idea_19.png" height="300" width="400">   | <img src="Linear Regression/img/idea_20.png" height="300" width="400"> 
<img src="Linear Regression/img/idea_21.png" height="300" width="400">   | <img src="Linear Regression/img/idea_22.png" height="300" width="400"> 
<img src="Linear Regression/img/idea_23.png" height="300" width="400">   | <img src="Linear Regression/img/idea_24.png" height="300" width="400"> 

## Assumptions
* Linear relationship
Linear regression needs the relationship between the independent and dependent variables to be linear.<br/>
<b>Scatter plot</b>

* Multivariate normality
The linear regression analysis requires all variables to be multivariate normal.<br/>
<b>QQ plot</b>

* No or little multicollinearity
Linear regression assumes that there is little or no multicollinearity in the data.  Multicollinearity occurs when the independent variables are too highly correlated with each other.<br/>
<b>Correlation matrix</b>


* No auto-correlation
Autocorrelation occurs when the residuals are not independent from each other.  For instance, this typically occurs in stock prices, where the price is not independent from the previous price.


* Homoscedasticity
The residuals are equal across the regression line.<br/>
<b>Scatter plot</b>


# Evaluation Metrics 
## Mean Square Error(MSE)/Root Mean Square Error(RMSE)
MSE is calculated by the sum of square of prediction error which is real output minus predicted output and then divide by the number of data points.

Root Mean Square Error(RMSE) is the square root of MSE. It is used more commonly than MSE <b>because firstly sometimes MSE value can be too big to compare easily. </b> Secondly, MSE is calculated by the square of error, and thus <b>square root brings it back to the same level of prediction error and makes it easier for interpretation.</b>

## Mean Absolute Error(MAE)
Mean Absolute Error(MAE) is similar to Mean Square Error(MSE). However, instead of the sum of square of error in MSE, MAE is taking the sum of the absolute value of error.

## R2
<img src="Linear Regression/img/R2_1.png" height="300" width="400">  | <img src="Linear Regression/img/R2_2.png" height="300" width="400">
------------- | -------------
<img src="Linear Regression/img/R2_3.png" height="300" width="400">  | <img src="Linear Regression/img/R2_4.png" height="300" width="400">
<img src="Linear Regression/img/R2_5.png" height="300" width="400">   | <img src="Linear Regression/img/R2_6.png" height="300" width="400"> 
<img src="Linear Regression/img/R2_7.png" height="300" width="400">   | <img src="Linear Regression/img/R2_8.png" height="300" width="400"> 
<img src="Linear Regression/img/R2_9.png" height="300" width="400">   | <img src="Linear Regression/img/R2_10.png" height="300" width="400"> 


# Conclusion
R Square/Adjusted R Square is better used to explain the model to other people because you can explain the number as a percentage of the output variability. MSE, RMSE, or MAE are better be used to compare performance between different regression models. However, it makes total sense to use MSE if the value is not too big and MAE if you do not want to penalize large prediction errors.
