# 2020_Investments
Please see the main Ipynb for my 2020 investments. The notebook calculates the return of 10 different strategies from the Beginning of 2019 to August of 2020.
These returns are benchmarked against both the S&P500 (SPY etf) and the NASDAQ100 (QQQ etf).
The strategies examined include the following:
- Minimum Variance
- Buy and Hold
- Equally Weighted Portfolio
- Maximum Sharpe Ratio Portfolio
- Equal Risk Contribution or Risk Parity Portfolio
- Robust Optimization Portfolio with the target return set to the Maximum return portfolio
- The portoflio that lies at the 25% point on the Efficient Frontier
- The Portfolio that lies at the 50% point on the Efficient Frontier
- The Portfolio that lies at the 75% point on the Efficient Frontier

A one month holding period and one month look back is used on a daily basis to detemrine the prices for which the program optimizes on.
It should be noted that the program makes use of IBM's CPLEX optimizer solver. A different computational optimizer could be used but it would require updates to the source code.
Efficient Frontier is calculated through brute force plotting of 1,000,000 random portfolios. The positions of interest on the Efficient Frontier (25%, 50%, and 75% of variance) are determined by finding the highest return for the given variance.

As can be seen the perfromance of the Portfolios varies widely, but the ERC portfolio is of particular interest.
