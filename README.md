# Risk Calculation using Backward Elimination Algorithm in Life Insurance
Here the python code contains implementation of backward elimination algorithm used for dimensionality reduction for improving the performance of risk calculation in life insurance industry. Though this experiment was performed on life insurance dataset publicly available on kaggle.com, the method is quite useful for dimensionality reduction on various domain as well.

  Backward elimination is the method of multiple linear regression and here it is used with Adjusted R squared. If Adjusted R squared values start decreasing, we should stop building model because of the higher probability of loosing significant relationship between maximum possible combination of independent variables and risk as a single dependent variable. 
  
  Also, according to alternative hypothesis of multiple linear regression models, there is a significant relationship between risk dependent variable (last column in the dataset) and independent variables( all column except last in the dataset provided). Hence according to alternative hypothesis, if we can figure out important correlation between dependent and maximum possible combination of independent variables, we will accept it and try to build a model rejecting the null hypothesis saying that there is not a significant relationship between risk dependent variable and single/combination of indpendent varible. 
  
  For this analysis I checked the p-value of statistical analysis for all independent variables. If the highest p-value obtained is greater than statistical significance ( 5% or 1%), I would eliminate that highest p-value variable from the analysis. Run the model of multiple linear regression one more time using all predictors excluding the predictor which has p-value greater than significance level until I found the highest p-value predictor whose p-value is equal to or less than significance level. This is the process of backward elimination. 
  
  I used the dataset of Prudential Life Insurance Assessment available in Kaggle.com for this analysis. We can easily check increment in accuracy for machine learning models, thanks to the Adjusted R square. 
  
  The significant fact obtained through this analysis is that accuracy of some machine-learning models increases with reducing unimportant features. Code only shows the execution of random forest demonstration. You can easily check the difference between accuracy of the model with including all features and eliminating unimportant features from backward elimination algorithm and Adjusted R squared trick.
  The result I got indicates that backward elimination is useful measure when used with Adjusted R squared trick to figure out important features for dependent variables. 
  
  If you want to learn more about this analysis or want to check the results I get from various and different models feel free to contact me at email address is hiwaseva@rknec.edu. I personaly believe that it will be more fun to check and run different machine learning and deepl learning technologies and validate the reuslt I obtained.
