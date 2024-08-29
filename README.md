# Geometric-Brownian-Motion-for-Stock-Market-Prediction
Geometric Brownian Motion for Stock Market Prediction
# Introduction
Brownian motion is a fundamental concept in stochastic processes, reprenting the random movement of particles, as first observed by botanist Robert Brown. This random behavior is mathematically modeled as a continuous-time stochastic process, ccharacterized by unpredictability. In finance, Brownian motion forms the basis for modeling the random fluctuations of asset prices over time. 
Geometric Brownian Motion (GBM) extends this idea to financial modeling, where it is used to represent the stochastic behavior of stock prices. GBM has both a deterministic trend (drift) and a random component (volatility), thus capturing the features of a real-world dynamic. GBM represents a mathematical foundation for option pricing models such as Black-Scholes, risk management strategies and simulation of asset prices.
The mathematical formulation of GBM is expressed by the following equation:\
dS_t = μ * S_t * dt + σ * S_t * dW_t

Where:

- `S_t` is the asset price at time `t`.
- `μ` is the drift coefficient (expected return).
- `σ` is the volatility coefficient (standard deviation of returns).
- `dW_t` is the increment of a Wiener process (standard Brownian motion).
## Explanation
- Drift term (`μS_tdt`): This term represents the expected deterministic growth of the asset price. It suggest that over the time interval `dt`, the asset price is expected to change by a factor of `μS_tdt`.
- Volatibility term (`σS_tdW_t`: This term represents the randomness (or noise) in the asset's price movement. That uncertainty is proportional to the current price level `S_t` and scaled by the volatility (`σ`). The term `dW_t` represents the random component, modeled as a Brownian motion.

To conclude, here as the key characteristics of GBM:
- Models the Continuous and random Motion (fluctuation) of an asset's price over time.
- The model assumes that the logarithm of the asset price is normally distributed (the asset price follows a log-normal distribution).
- Insures that the asset price remains non-negative by modeling the price as positive quantity that grows over time.
  
# Analysis and Results
The simulation using GBM model generated paths for stock prices over a year. The paths show the randomness and variability in financial markets. The paths simulated show both upward and downwoard trends, showcasing the stochastic nature of stock prices. As the simulation progressed, the paths have shown higher volatility which is a characteristic of GBM where variance grows over time.
![image](https://github.com/user-attachments/assets/7e095a9b-d621-4e54-85ac-7cd6806c34e8)

![image](https://github.com/user-attachments/assets/63c01d4c-222c-461c-9d60-535d302761de)

The histogram of the final stock prices form the simulations shows largely a normal distrbution, centered around the initial stock price. However, there's a probability of higher and lower final prices.
![image](https://github.com/user-attachments/assets/2bdc8f3f-b1d1-4093-b010-2744efdfdbe9)

When comparing the simulated stock prices paths (using non-tuned parameters) with the historical AAPL stock prices, it becomes evident that the simulated paths have volatility but not enough precision with real-world trends. The historical prices (red line) lie within the range of the simulated paths but could be improved for accuracy.
![image](https://github.com/user-attachments/assets/d0813f72-855a-4005-8ea4-a64132cff2b7)

After tuning the parameters (both drift and volatility) based on historical AAPL data, the GBM simulations shows a closer alignmenent with AAPL historical stock prices. The estimated drift of -0.3398 indicates a sligh negative trends. The volatility of 0.3561 captures the level of fluctuation seen in the real market data. This demonstrates that parameter tuning can significantly better the predictive power of the model.
![image](https://github.com/user-attachments/assets/3c60ff59-64ea-48be-81cd-3c1e2faf6377)

