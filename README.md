# Erdos institute Quant Finance project

In this repository are the four mini-projects required to complete the Erdos Institute's Quantitative Finance bootcamp of summer 2025.

### Project 1

I construct two "potentially profitable" portfolios, one "higher risk" and the other "lower risk". For the purposes of this project, I measure potential profitiability (very crudely) by the historical annualised expected value of stock returns. On the other hand, risk will be quantified by volatility, i.e. the annualised standard deviation of historical daily log returns. I minimise the volatility of a potential portfolio of stocks by minimising the quadratic form associated with the (sample) covariance matrix over all weight vectors with non-negative entries that sum to 1. The volatility of the optimal portfolio is less than the volatility of each individual stock, showing the value of diversification for minimising risk. 

### Project 2

In many financial mathematical models, it is common to assume that the log returns of a stock or index are normally distributed. I use the D'Agostino and Pearson test to investigate this assumption for some historical stock data. I take 4 randomly chosen stocks and analyse their price data for the previous 4 years. I show that the null hypothesis that log returns are normally distributed can be rejected in certain historical time periods, but not rejected in others. Thus, the models that use this assumption are not always appropriate.

### Project 3

I examine two of the Greeks of options pricing: _delta_ (sensitivity of an option's price with respect to spot price) and _theta_ (time sensitivity). In a toy example with a given strike (K) and volatility (sigma), I plot the price and delta of a call and put as a function of spot price (S0), and the theta and price of the same call and put as a function of time to expiration (tau) and time (t). I recover the well known facts about the behaviour of the Greeks. 

### Project 4

In this final project, I examine the effect of a non-constant volatility on the distribution of profits of selling a call, using a hedging strategy that hedges against sigma, i.e. mitigates against the risk of loss due to changes in volatility. I use the _n_-step Heston model to simulate the path of a stock price. The hedging strategy will then be _vega_ neutral -- where the vega of an option's price is it's rate of change with respect to sigma -- in the sense that at each discretised time step, the vega of the overall portfolio will be zero. In order to undertake such a vega neutral strategy, the instrument used to hedge against our initial short position in selling a call will be a long position in a call of the same time to expiration but with strike 2 x (spot price) - (strike price). This strategy hedges against the risk of serious loss in the short call through the potential of immense gain (although smaller in magnitude that the loss of the sold call due the differing strike price) of the bought call. I also produce some code that uses Monte Carlo simulation to compute (approximately) the vega of an option's price.
