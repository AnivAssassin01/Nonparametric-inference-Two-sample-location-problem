# 2-Sample Location Problem: Non-Parametric Inference

## 📖 Overview
[cite_start]This project provides an in-depth exploration of the Two-Sample Location Problem using non-parametric statistical methods[cite: 1840, 1855]. [cite_start]The core focus is on the **Mann-Whitney U (Wilcoxon Rank Sum) statistic**, evaluating its theoretical properties, practical robustness, and efficiency compared to classical parametric tests (like the t-test)[cite: 1883, 3458, 3459]. 

[cite_start]Through extensive Monte Carlo simulations, this study analyzes how the test behaves under standard conditions, extreme distribution shapes, and scenarios where foundational assumptions fail[cite: 1848, 1850, 1997]. [cite_start]It also introduces a modern application of rank-based statistics in high-dimensional feature spaces ($p \gg n$)[cite: 1852, 3571].

## 🔍 Key Investigations

### 1. Null Distribution & Distribution-Free Properties
* [cite_start]**Exact and Asymptotic Distributions:** Examines the exact combinatorial probability mass of the statistic for small samples and its convergence to normality as sample sizes increase[cite: 1848, 1928, 1937].
* [cite_start]**Distribution-Free Guarantee:** Demonstrates that under the null hypothesis, the test's behavior is independent of the underlying continuous population distribution (e.g., Normal, Cauchy, Beta, Chi-square)[cite: 1928, 1997, 2054].

### 2. Assumption Violations & Robustness
* [cite_start]**Discrete Data & Ties:** Investigates how discrete distributions (e.g., Poisson, Binomial, Geometric) cause ties, which inherently break the exact distribution-free property and result in a conservative leftward shift of the null distribution[cite: 1850, 2848, 2896].
* [cite_start]**Dependent Samples:** Analyzes the behavior of the Mann-Whitney statistic when samples are drawn from bivariate distributions (correlated data), showing how within-sample dependence systematically depresses the test statistic[cite: 1850, 2958, 2977].
* [cite_start]**Imbalanced Sample Sizes:** Tests the limits of asymptotic normality when the proportional sample size condition ($m/N \to \lambda_0$) is heavily violated or oscillates[cite: 1848, 2397, 2409].

### 3. Power, Efficiency, and Estimation
* **Power Curves:** Evaluates the empirical power functions under right-tailed, left-tailed, and two-tailed alternatives across various distributions. [cite_start]It highlights the test's high Asymptotic Relative Efficiency (ARE) under heavy-tailed distributions like Laplace and Cauchy[cite: 1850, 3050, 3055, 3069].
* [cite_start]**Hodges-Lehmann Estimator:** Explores the point estimator derived by inverting the Mann-Whitney test, demonstrating its near-unbiasedness, consistency, and robustness to outliers[cite: 1850, 2753, 2783].

### 4. Parametric vs. Non-Parametric Testing
* [cite_start]Compares the Mann-Whitney U test against Welch's t-test[cite: 1852, 3463].
* [cite_start]Demonstrates that while the tests perform almost identically under Normal distributions, the Mann-Whitney test vastly outperforms the t-test in the presence of heavy-tailed noise (e.g., Cauchy) and offers distinct advantages under heteroscedasticity[cite: 3251, 3255, 3544, 3561].

### 5. High-Dimensional Application ($p \gg n$)
* [cite_start]Applies the Mann-Whitney-based max-statistic to high-dimensional datasets where classical methods like Hotelling's $T^2$ fail due to covariance matrix singularity[cite: 1852, 3571, 3572].
* [cite_start]Proves the utility of rank-based testing for **Sparse Signal Detection** in heavy-tailed noise, with direct applications to bioinformatics (gene expression) and financial risk management[cite: 3600, 3641, 3647, 3651].

## 🛠️ Methodology & Tools
* [cite_start]**Statistical Methods:** Mann-Whitney U Test, Wilcoxon Rank Sum, Hodges-Lehmann Estimation, Welch's T-Test, Monte Carlo Simulations, Max-Type Statistics[cite: 1883, 2699, 2753, 3467, 3593].
* [cite_start]**Distributions Simulated:** Normal, Cauchy, Laplace, Logistic, Exponential, Poisson, Binomial, Geometric, Negative Binomial[cite: 1997, 2070, 2803, 2851].
* [cite_start]**Environment:** Computations, Q-Q plots, density estimations, and power curves generated programmatically (using R/simulation environments)[cite: 2220, 2805, 3064].

## 👥 Authors
* [cite_start]**Aniv Mazumder** * **Koushan Saha** * **Sanjhali Parmar** *Project Report for Non-Parametric Inference, Indian Statistical Institute (M.STAT, 2nd Semester) - Under the guidance of Prof. Isha Dewan*[cite: 1838, 1839, 1841, 1843, 1846].
