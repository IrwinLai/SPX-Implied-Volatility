## SPX Implied Volatility

### Content

1. Using Newton's method to calculate implied volatility of SPX's various options.
2. Plot implied volatility to see whether there is a implied volatility smile

### Data
- SPY index, Sept 2019 - Nov 2019, from Bloomberg (SPY index was around 3000 during this time)
- Call and Put option, strike price from 2500 to 3500

### Solution

use two functions : BSM: to calculate the option's price, and IV: to get implied volatility by Newton's method.

### Conclusion & Analysis
1. Useing this way, the implied volatility is higher than the IV Bloomberg calculated. May becasue BSM model assume constant volatility, so we should use better model to price. And Bloomberg may use advanced way, like variance swap, to get IV.
2. In the deep out of money part, the implied volatility is much higher than the real one. The reason is because the deep out of money options were lack of liquidity. So I use the previous one to replace, which make the results higher.

![](https://tva1.sinaimg.cn/large/0082zybpgy1gbr3l4hzdrj31be0kk3zb.jpg)

#### BSM

<img src="https://tva1.sinaimg.cn/large/006y8mN6gy1g85derir5uj30x20lggnb.jpg" width = "55%" />

- s - Current price of the underlying
- k - Strike price
- t - Time to experiation in years
- r - Anual risk-free interest rate, SOFR
- sigma - volatility
- cp - Call or Put
