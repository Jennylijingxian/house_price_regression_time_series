# Regression and Time Series Analysis of House Price  
- **Project 1: How do house condition related variables influence house price in Seattle?**    
 
  - Data: 
    - Source: https://www.kaggle.com/shree1992/housedata
    - Dimension: 1573 records of house price, 18 featuers   
  - Contents:
    - Linear regression model
      - Exploratory analysis
      - Model setup and preliminary evaluation (Normality and fitted value vs. residual)
      - Drop influential points by combining hat matrix, internal and external residual, DFFITS, cook’s distance and model reevaluation
      - Model selection:
        - Stepwise
        - Best subset regression
        - Using Mallow’s Cp, AIC, BIC, adjusted R square
      - Compare best model in stepwise and best subset regression. Test on non-equal variance, multicollinearity and solve related problems
      - Choose the final model based on the above criteria and do the model evaluation
    - Logistic model
      - Test on the best model of former linear regression and drop/add variables if necessary
      - Begin with the full model to remove or add variables for logistic

- **Project 2: Predict California monthly median sold price from 2016/1 - 2017/8 given data on previous mortage rate, rental price and sold price.**
  - Data descirption:   
  The Zillow dataset (modified) recorded Jan 2004- Dec 2015 monthly median sold price for housing in California, Jan 2004-Aug 2017 monthly median mortgage rate, Jan 2004-Aug 2017 monthly unemployment rate, and Jan 2010- Aug 2017 median monthly rental price.  
  - Summary:  
  Used SARIMA, SARIMAX, Exponential Smoothing to make predictions and further imputed missing values with median, ARIMA and VAR. 
  - Conclusion:   
    - ARIMA imputation has best performance. 
    - VAR is not good at capturing seasonality.
    - TES predicts very well in the short term.
