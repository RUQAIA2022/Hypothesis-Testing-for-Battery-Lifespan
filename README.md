# Hypothesis-Testing-for-Battery-Lifespan
A company claims their car batteries last 2 or more years on average. An engineer suspects the average is actually less than 2 years. With a sample of 10 batteries showing:

Sample mean (x̄) = 1.8 years

Sample standard deviation (s) = 0.15 years

Sample size (n) = 10

We need to:
(a) State hypotheses
(b) Test at 99% confidence level
(c) Implement in Python

(a) State the null and alternative hypotheses
Null Hypothesis (H₀): μ ≥ 2 years (company's claim)

Alternative Hypothesis (H₁): μ < 2 years (engineer's suspicion)

This is a one-tailed t-test because:

We're testing "less than" specifically
We have a small sample (n=10) with unknown population standard deviation

(b) Hypothesis Test at 99% Confidence Level
Given:

Sample mean (x̄) = 1.8
Hypothesized mean (μ₀) = 2
Sample standard deviation (s) = 0.15
Sample size (n) = 10

Confidence level = 99% (α = 0.01)

steps:
1.
Calculate the t-statistic:
t = (x̄ - μ₀) / (s/√n)
t = (1.8 - 2) / (0.15/√10)
t = -0.2 / 0.04743
t ≈ -4.216

2.Find the critical t-value:
-Degrees of freedom (df) = n - 1 = 9
-One-tailed test (left-tailed)
-t-critical for α=0.01, df=9 ≈ -2.821

3.Compare t-statistic to t-critical:
Our t-statistic (-4.216) < t-critical (-2.821)
The test statistic falls in the rejection region

Conclusion:
We reject the null hypothesis at the 99% confidence level.
There is statistically significant evidence that the average battery lifespan is less than 2 years.
