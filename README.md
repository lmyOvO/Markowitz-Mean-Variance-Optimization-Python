# Markowitz Mean-Variance Optimization Using Python

## Background
Portfolio optimization is the process of determining the allocation of funds to a set of assets which yields the maximum performance. Performance can be thought of as maximizing return, minimizing risk, or maximizing the risk adjusted return (Sharpe ratio).

Markowitz (1959) mean-variance optimization (MVO) has been the standard for efficient portfolio construction for almost fifty years. MVO lowers the cumulative risk of a portfolio by blending anti- correlated data since equities which are positively correlated in the long term but anti-correlated in the short term cumulatively have equal returns but lower volatility. For a given set of equities, computing the MVO portfolio for the range of possible portfolio returns the efficient frontier. Thus, the efficient frontier is the set of optimal portfolios that offer the highest expected return for a defined level of risk or the lowest risk for a given level of expected return.

The drawback to conducting MVO on its own is that the algorithm is highly affected by sampling error in the input data. As well as being sensitive to uncertainty in risk-return estimates.

Resampling efficiency optimization and rebalancing technology (RE), developed by Michaud in 1998, introduces Monte Carlo resampling and bootstrapping methods into MV optimization. The portfolio built after the resampling method is applied is generally more stable, realistic, and investment efficient than MVO alone. Each resampled dataset will create a new set of Markowitz efficient portfolios to form a new efficient frontier. The resampled efficient frontier lies below the classical MV frontier. RE optimization expects less return and restricts risk to a narrower range. RE optimization can be thought of as a constraint which lowers in-sample expectations and improves out-of-sample performance.

## Steps to perform:
Given a data set of monthly closing prices for 25 assets from Jan 1st, 2018, to Dec 1st, 2020 (in-sample) and closing prices for the same assets in 2021 (out-of-sample), complete the following:

1.  Load and clean data, in-sample data (2018-2020) and out-of-sample data (2021). From the in-sample data, compute the classical Markowitz and resampled Markowitz frontiers

    a) Import necessary libraries and dataset, compute the matrix of monthly returns 

    b) Compute the covariance matrix and means of the percent change matrix 

    c) Solve for the minimum variance portfolio 

    d) Solve for the maximum variance portfolio 

    e) Compute the classical Markowitz efficient frontier 

    f) Compute the resampled efficient frontier 
    
2. Using the frontiers, compute three portfolio weights (minimum variance, maximum return, and Sharpe ratio) along both the classical and resampled frontiers. Compare the performance of each of these portfolios on the out-of-sample data. Assume a total investment of $1000 and a risk-free- return of 0.2% monthly (0.002). 

    a) On the classical efficient frontier, find the minimum variance, maximum return, and Sharpe ratio portfolio weights
    
    b) On the resampled efficient fronter, find the minimum variance, maximum return, and Sharpe ratio portfolio weights 
    
    c) For each of the 6 portfolios, calculate the expected return on the 2022 (out-of-sample) data for a $1000 investment 

3. Plot the classical and resampled efficient frontiers 

4. Plot the portfolio compositions for classical and resampled frontiers

5. Discuss the findings from comparing the performance of all 6 portfolios and from observing the
graphs from questions 3 & 4
