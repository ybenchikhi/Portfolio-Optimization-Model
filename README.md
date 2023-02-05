# Portfolio-Optimization-Model
Portfolio optimization model using Python and the scipy library, which helps optimize the portfolio for a given set of assets and constraints

The code I developed is a portfolio optimization model using Python and the scipy library. The goal of the model is to optimize the portfolio for a given set of assets and constraints to help an investor with low risk tolerance to project for a return over a year with a 100k initial starting injection.

The first step I took was to import the necessary libraries, specifically the scipy library's minimize function, which is used to optimize the portfolio. Then I defined the asset returns, covariance matrix, and risk-free rate. I had to make assumptions about the expected returns, volatility and covariance of low-risk assets as per the requirement of the low risk tolerance investor.

Next, I defined the optimization function, which is the negative sharpe ratio, which is a measure of risk-adjusted return. This function takes in the weights of the assets in the portfolio and calculates the portfolio return and volatility. The goal of the optimization is to maximize this ratio.

After that, I defined the constraints of the optimization, which include the sum of the weights being equal to 1 and the weights being greater than or equal to 0. I also defined the bounds of the weights as being between 0 and 1.

I initialized the weights with equal values for all assets and then used the minimize function to optimize the portfolio. I passed the optimization function, initial weights, constraints, and bounds as arguments to the minimize function.

Lastly, I calculated the optimized portfolio return and volatility using the optimized weights obtained from the minimize function and the investment amount.

The toughest obstacle I faced during development was to make assumptions about the expected returns, volatility and covariance of low-risk assets as there is no clear information available in the real world. In practice, there are various other factors that should be considered for portfolio optimization such as any specific investment constraints, taxes and transaction costs.

To overcome this challenge, I had to do some research and gather information from various sources, and also try different sets of assumptions to check their impact on the final results.
