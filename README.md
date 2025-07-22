# Landing Page A/B Test – CTR Uplift Analysis

This project analyzes the effectiveness of two landing page designs using real-world-like A/B testing data from Kaggle. The goal is to determine whether the new design leads to a statistically and practically significant improvement in user click-through rates (CTR).

---

## Objective

To evaluate whether a new landing page leads to a **higher conversion rate** compared to the existing design, using:
- A/B testing methodology
- Hypothesis testing (Z-test)
- Power analysis
- Confidence interval interpretation
- Practical significance assessment

---

##  Dataset

- Source: [Kaggle – Lunar Tech A/B Testing Dataset](https://www.kaggle.com/datasets/andrsulloa/lunar-tech-case-study-ab-testing)
- Contains 20,000 users split into `control` and `experiment` groups.
- Each record includes:
  - `user_id`
  - `group` (control/experiment)
  - `landing_page` (old/new)
  - `click` (1 = clicked, 0 = did not click)

---

##  Methodology

1. **Data Cleaning & Validation**
   - Checked group assignment balance.
   - Ensured no user overlap between groups.

2. **Exploratory Analysis**
   - Visualized group sizes.
   - Computed raw CTRs for each group.

3. **Hypothesis Testing**
   - Null Hypothesis (H₀): No difference in conversion.
   - Performed a two-sample Z-test.
   - Built a 95% Confidence Interval.

4. **Power Analysis**
   - Estimated required sample size for a Minimum Detectable Effect (MDE) of 2%.
   - Used `statsmodels` for power calculation.

5. **Practical Significance Check**
   - Assessed if the observed uplift was not just statistically significant but also meaningful for business rollout.

---


---

##  Tech Stack

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- SciPy, statsmodels

---




