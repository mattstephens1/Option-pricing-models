# Option-pricing-models
This project uses both the Black-Scholes closed-form model and Monte Carlo simulation. It demonstrates both quantitative finance skills including numerical methods and risk-neutral valuation.

This notebook contains:
- Implementing the Black-Scholes and Monte Carlo simulations
- Analysed the convergence behaviour, through comparing both models
- Computed Greeks to understand hedging and risk management


## Black-Scholes model
Uses the formula:




<img width="424" height="143" alt="image" src="https://github.com/user-attachments/assets/092624c6-de5f-4a2c-8a60-fb041a732883" />

## Monte Carlo Simulation
Estimates the option price by simulating possible future stock prices under geometric Brownian motion (GBM):

<img width="331" height="40" alt="image" src="https://github.com/user-attachments/assets/2829b30b-074f-4989-ad63-86da2536a3f3" />

## Convergence Analysis
Ran the Monte Carlo simulation with increasing numbers of paths and compared it with the Black-Scholes price. Also ran the Monte Carlo simulation multiple times to calculate the average error of running a different number of paths.

## Greeks: Delta and Gamma
Delta - the sensitivity of the option price to small changes in the underlying stock
Gamma - the rate of change of Delta
These are both crucial for hedging and understanding why rebalancing is required to manage risk

## Key results
- The Monte Carlo simulation converges to the Black-Scholes price as number of trials is increased
- Delta follows S-shaped curve between 0 and 1
- Gamma peaks near-the-money, highlighting the point when frequent re-hedging is required
