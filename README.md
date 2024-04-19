## Washu Career Development Center Website Pop-up A/B Test

### For detailed calculation and outcome, please view the jupyter notebook file. ###

## Washu Career Development Center Website Pop-up A/B Test

### Experiment Overview
**Experiment Name:** "Study Plan" Pop-up A/B Test

**Conducted by:** Washu Career Development Center Course Website Team

**Objective:**
- Introduce a "Study Plan" pop-up on the homepage to potentially increase the course completion rates among students. Randomly divide users into experimental and control groups.
- Collect data from the website backend over a 1-month period, acquiring over 1000 data points regarding cookie counts and attendance rates from both groups.
- Set clicks and pageviews as invariant metrics; conversion and completion rates as experimental metrics. Determine the right pivot quantities to construct confidence intervals and assess the significance of changes.

### Metrics:
- **Invariant Metrics:** Clicks (`Ck`) and pageviews (`Cv`), expected to remain unchanged and serve as sanity checks.
- **Evaluation Metrics:** Conversion rates (`Cr`) and completion rates (`Cm`), which are essential for measuring the experiment's success.

### Outcome:
- Analysis indicated no significant impact on completion rates due to the pop-up. Recommendation was made to the Career Center to consider discontinuing the pop-up based on these results.

### Analysis Summary:
The process of analysis involved the following steps:

1. **Baseline Value Estimation:**
   Estimators for metrics were calculated to understand their behavior before the change.

2. **Standard Deviation Estimation:**
   We calculated the Standard Deviation to gauge the variability of metrics, essential for sample size calculations and confidence intervals.

3. **Sample Size Sizing:**
   Determined the minimum number of samples required for the experiment to have enough statistical power and significance.

4. **Sanity Checks:**
   Verified the experiment's proper execution and the correct collection of data through sanity checks for invariant metrics.

5. **Effect Size Analysis:**
   Examined the differences in evaluation metrics between control and experiment groups to assess both statistical and practical significance.

### Key Formulas and Outputs:

- **Variance Calculation for Binomial Distribution:**
  `SD = sqrt(p * (1-p) / n)`
  Where `p` is the probability of success, and `n` is the sample size.

- **Z-score Calculation:**
  `Z = norm.ppf(1-alpha/2)`
  Determines the critical value at the desired confidence level.

- **Confidence Interval for observed conversion rate (`p_hat`):**
  `CI = [p_hat - ME, p_hat + ME]`
  Where `ME` is the margin of error calculated as `Z * SD`.

### Results from Calculations:
- **Gross Conversion SD:** 0.0202
- **Retention SD:** 0.0549
- **Net Conversion SD:** 0.0156

### Detailed Analysis of Results:
#### Sanity Checks:
- Pageviews and clicks matched expected distributions, passing sanity checks.
- Click-through-probability on the "Study Plan" pop-up fell within the expected range.

#### Effect Size Tests:
- Gross Conversion had a statistically significant decrease, suggesting fewer students enrolled after seeing the pop-up.
- Net Conversion did not show a statistically significant decrease, indicating that the pop-up did not deter students from continuing past the free trial.

#### Practical Significance:
- While Gross Conversion met the practical significance criteria (dmin = 0.01), Net Conversion did not (dmin = 0.0075).
- The decrease in Gross Conversion was significant enough to suggest the pop-up may deter some students from enrolling.


