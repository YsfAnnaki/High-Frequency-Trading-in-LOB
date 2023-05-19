# High-Frequency-Trading-in-LOB

[Youssef ANNAKI](https://www.linkedin.com/in/youssef-annaki-a91ab5192/)

Project done from February 2022 to April 2022.
## Summary

The goal of this work is to study a high frequency market-making strategy inspired from the work of Marco Avellaneda & Sasha Stoikov in High-frequency trading in a limit order
book (2006). Given the current state of the limit order book, we introduce the notion of the "indifference price" and we determine the optimal spread and bid/ask orders to quote on the order book based on a stochastic control approach. In order to analyze the performance of the market_making strategy, we use 1 day worth of granular order book data and tick data for different stocks (AXA, BNP, CARREFOUR, LVMH, TOTAL) and we build and implement a market-making strategy based on the findings of Marco Avellaneda & Sasha Stoikov.
This work focuses on the following subjects:
- General formulation of the Stochastic Control framework and the definition of the Hamilton-Jacobi-Bellman equation related to this stochastic control problem (for finite & infinite trading time horizon):

$` u(s,x,q,t) = sup_{(\delta^a_t)_t, (\delta^b_t)_t \in \mathcal{A}}\mathbb{E}_t[-exp(-\gamma(X_T + q_T S_T))] `$

- Derivation of the exact and approximate solution (optimal spreads to quote) to the stochastic optimization problem and the study of their temporal asymptotic behaviour:

$` \delta^b_t \approx \frac{1}{\gamma}ln(1+\frac{\gamma}{k})+\frac{1+2q}{2}\gamma \sigma^2 (T-t) `$

$` \delta^a_t \approx \frac{1}{\gamma}ln(1+\frac{\gamma}{k})+\frac{1-2q}{2}\gamma \sigma^2 (T-t) `$
            
- Backtesting of the market-making strategy on high-frequency data and defining two slightly different strategies (posting optimal limit orders using the mid-price as a reference for the first strategy and the indifference price for the second one).

## Some Results

### Optimal Bid/Ask quotes
![image](https://github.com/YsfAnnaki/High-Frequency-Trading-in-LOB/assets/134018406/ee4a0a75-f363-427e-a0a3-87152348fe2f)

### Optimal Spread
![image](https://github.com/YsfAnnaki/High-Frequency-Trading-in-LOB/assets/134018406/d6f9615e-7e79-4d24-b95a-f77c2c1e5631)

### Strategy backtest P&L, Inventory and optimal quotes evolution

![image](https://github.com/YsfAnnaki/High-Frequency-Trading-in-LOB/assets/134018406/ef74587f-f7a2-4eb0-acf0-f652dfb5ba5d)




More details regarding the practical convergence rates findings can be found in the project report.

##

For any information, feedback or questions, please [Contact me](mailto:annaki.youssef@gmail.com?subject=[GitHub]%20Source%20Han%20Sans)

