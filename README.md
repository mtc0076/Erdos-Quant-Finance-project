# Erdos institute Quant Finance project

In this repository are the four mini-projects required to complete the Erdos Institute's Quantitative Finance bootcamp of summer 2025.

### Project 1
I construct two "potentially profitable" portfolios, one "higher risk" and the other "lower risk". For the purposes of this project, I measure potential profitiability (very crudely) by the historical annualised expected value of stock returns. On the other hand, risk will be quantified by volatility, i.e. the annualised standard deviation of historical daily log returns. I minimise the volatility of a potential portfolio of stocks by minimising the quadratic form associated with the (sample) covariance matrix over all weight vectors with non-negative entries that sum to 1. The volatility of the optimal portfolio is less than the volatility of each individual stock, showing the value of diversification for minimising risk. 

### Project 2

In many financial mathematical models, it is common to assume that the log returns of a stock or index are normally distributed. I use the D'Agostino and Pearson test to investigate this assumption for some historical stock data. I take 4 randomly chosen stocks and analyse their price data for the previous 4 years. I show that the null hypothesis that log returns are normally distributed can be rejected in certain historical time periods, but not rejected in others. Thus, the models that use this assumption are not always appropriate.

### Project 3

I examine the 


### Project 4

And here, we do more blah
