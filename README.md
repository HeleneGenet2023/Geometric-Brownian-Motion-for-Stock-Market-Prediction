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
  
# Results

# Analysis
