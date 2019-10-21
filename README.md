## SPX Implied Volatility

### Content

1. Using Newton's method to calculate implied volatility of SPX's various options.
2. Plot implied volatility to see whether there is a implied volatility smile

### Solution

we need two functions : BSM, and IV

#### BSM

<img src="https://tva1.sinaimg.cn/large/006y8mN6gy1g85d5sj45xj30ti0fq75r.jpg" width = "55%" />

- s - Current price of the underlying
- k - Strike price
- t - Time to experiation in years
- r - Anual risk-free interest rate, SOFR
- sigma - volatility
- cp - Call or Put
