# Monte Carlo Simulation – Euler–Maruyama Scheme  

## Project Overview  
This project implements **Monte Carlo (MC) methods** for simulating stochastic processes in finance, using the **Euler–Maruyama (EM) scheme**. The notebook demonstrates how stochastic differential equations (SDEs) can be discretized and simulated numerically to estimate option prices and analyze convergence properties.  

Monte Carlo methods are widely used in **quantitative finance** for:  
- Pricing derivatives (European, Asian, Barrier options)  
- Risk management and Value-at-Risk estimation  
- Stress testing and portfolio optimization  

The focus of this project is on **Euler–Maruyama**, a widely used numerical approximation for simulating SDEs such as **Geometric Brownian Motion (GBM)**, which underpins the Black–Scholes model.  

---

## Key Features  
- Implementation of the **Euler–Maruyama discretization**  
- Simulation of **Geometric Brownian Motion (GBM)** paths  
- Convergence analysis (numerical vs analytical solutions)  
- Monte Carlo option pricing framework  
- Clear explanations embedded in Jupyter cells  

---

## Theory Background  
An SDE of the form:  

\[
dX_t = \mu X_t \, dt + \sigma X_t \, dW_t
\]  

is approximated under Euler–Maruyama as:  

\[
X_{t+\Delta t} = X_t + \mu X_t \Delta t + \sigma X_t \sqrt{\Delta t}\, Z
\]  

where \( Z \sim \mathcal{N}(0,1) \).  
This allows us to numerically generate asset price paths and use them for pricing and risk analysis.  


