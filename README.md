# Optimization for Pair Trading
This project leverages the WRDS database to develop and refine a pair trading strategy using S&P 500 data from September 2, 2021, to January 10, 2023. Performance was calculated using total daily returns.

Our methodology utilized a multi-stage selection process. First, we applied a correlation filter to identify stock pairs with a coefficient exceeding 0.8. These candidates then underwent cointegration testing, narrowing the selection to 872 qualified pairs. Trading signals were generated based on the Z-score of the price spread for each specific pair.

In the final phase, we optimized the threshold coefficients using a one-year training window followed by a three-month backtest. By moving from fixed thresholds to optimized parameters, we increased the average three-month cumulative return from 2% to 13%, achieving a Sharpe Ratio of 1.7. This approach effectively identifies the specific pairs most conducive to the algorithm’s success.
