# Do Diets 1 & 2 Yield Different Growth? A data analysis for the farm industry

This project analyzes the **ChickWeight** dataset to compare 21-day growth for **Diet 1 vs Diet 2**. Growth is computed as weight on day 21 minus weight on day 0. Four Diet-1 chicks with missing day-21 values  are excluded, leaving **n₁ = 16** and **n₂ = 10**.

## Findings (brief)
- **Normality:** Both groups have likely a  distribution which is normal (Shapiro–Wilk, p > 0.05, Q-Q plots).
- **Mean difference:** **Welch’s t-test p = 0.2115**, **fail to reject the null hypothesis**. 
- **Confidence interval** : 95CI=[-23.3,98.8], 90CI=[-12.6, 88.2], they contain 0, which confirms Welch's t-test.  However they are large
  **Conclusion:** No statistically significant difference in 21-day growth between Diet 1 and Diet 2.

## How to run
1. Install deps from `requirements.txt` 
   ```bash
   pip install -r requirements.txt
