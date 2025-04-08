# Statistics Q&A Cheat Sheet

## 1. What is the difference between mean, median, and mode?
**Mean:** The average of all values.  
**Median:** The middle value in an ordered dataset.  
**Mode:** The most frequently occurring value.  
**Formulas:**  
- Mean: \( \bar{x} = \frac{\sum x_i}{n} \)  
- Median: Middle value (or average of two middle values if \( n \) is even).  
- Mode: Value with the highest frequency.  
**Example:** For \([2,3,3,5,7]\): Mean = 4, Median = 3, Mode = 3.

## 2. How do outliers affect the mean and median?
**Outliers:** Extreme values that deviate significantly from other observations.  
**Effect:**  
- Mean: Sensitive to outliers.  
- Median: Robust to outliers.  
**Example:** For \([1,2,3,4,100]\): Mean = 22, Median = 3.

## 3. What is the formula for calculating variance?
**Variance:** Measures spread around the mean.  
**Formulas:**  
- Population: \( \sigma^2 = \frac{\sum(x_i - \mu)^2}{N} \)  
- Sample: \( s^2 = \frac{\sum(x_i - \bar{x})^2}{n - 1} \)  
**Example:** For \([1,2,3,4,5]\), sample variance = 2.5.

## 4. What does a standard deviation of zero indicate?
**Standard Deviation:** Average distance from the mean.  
**If \( \sigma = 0 \):** All values are identical.  
**Example:** \([5,5,5]\) has \( \sigma = 0 \).

## 5. Explain the interquartile range (IQR) and its use.
**IQR:** \( Q3 - Q1 \), the middle 50% spread.  
**Use:** Detects outliers, summarizes spread.  
**Example:** \([1,3,5,7,9]\): IQR = 4.

## 6. What is skewness? Describe left-skewed and right-skewed distributions.
**Skewness:** Asymmetry in data.  
- Left-skewed: Tail on left (Mean < Median)  
- Right-skewed: Tail on right (Mean > Median)  
**Example:** Income is typically right-skewed.

## 7. How do you identify outliers using the IQR method?
**Outliers:** \( < Q1 - 1.5 \times IQR \) or \( > Q3 + 1.5 \times IQR \).  
**Steps:**  
1. Compute Q1 and Q3  
2. Calculate IQR  
3. Define bounds  
**Example:** For \([1,3,5,7,9]\): Outliers \(< -3\) or \(> 13\).

## 8. What is kurtosis, and how does it differ from skewness?
**Kurtosis:** Measures tail heaviness.  
**Skewness:** Measures asymmetry.  
- Leptokurtic: Heavy tails  
- Platykurtic: Light tails

## 9. What is the empirical rule (68-95-99.7 rule)?
**Rule:** In normal distribution:  
- 68% within \( \mu \pm \sigma \)  
- 95% within \( \mu \pm 2\sigma \)  
- 99.7% within \( \mu \pm 3\sigma \)

## 10. What is the difference between a population and a sample?
- **Population:** Entire group of interest.  
- **Sample:** Subset of population.

## 11. What is a percentile? How is it different from a quartile?
- **Percentile:** Value below which a % of data falls.  
- **Quartile:** 25th, 50th, 75th percentiles.

## 12. How do you calculate the coefficient of variation?
**Formula:** \( CV = \frac{\sigma}{\mu} \times 100\% \)  
**Example:** \( \sigma = 10, \mu = 50 \Rightarrow CV = 20\% \)

## 13. What is the difference between range and IQR?
- **Range:** Max - Min  
- **IQR:** Q3 - Q1  
- **Key:** IQR is robust to outliers.

## 14. What does a box plot show?
**Box Plot:** Visual summary showing:  
- Median  
- Quartiles  
- Outliers

## 15. What is the relationship between variance and standard deviation?
**Std. Dev. (\( \sigma \)) :** Square root of variance.  
**Formula:** \( \sigma = \sqrt{\sigma^2} \)

## 16. When would you prefer the median over the mean?
**Use Median:** For skewed or outlier-prone data.

## 17. What is the 5-number summary?
**Summary:** Min, Q1, Median, Q3, Max

## 18. How do you interpret a z-score?
**Z-score:** Number of SDs from mean.  
**Formula:** \( z = \frac{x - \mu}{\sigma} \)  
**Example:** \( z = 2 \Rightarrow 2 SDs above mean \)

## 19. What does a covariance of zero imply?
**Covariance = 0:** No linear relationship.

## 20. What is the difference between descriptive and inferential statistics?
- **Descriptive:** Summarizes data.  
- **Inferential:** Generalizes/predicts.

## 21. What is the trimmed mean, and when is it useful?
**Trimmed Mean:** Removes extremes before averaging.  
**Use:** Reduces outlier effects.

## 22. How does the geometric mean differ from the arithmetic mean?
- **Geometric Mean:** \( \sqrt[n]{x_1 x_2 \dots x_n} \)  
- **Arithmetic Mean:** Regular average  
**Use:** Multiplicative data (growth).

## 23. What is the harmonic mean, and where is it applied?
**Harmonic Mean:** \( HM = \frac{n}{\sum \frac{1}{x_i}} \)  
**Use:** Rates and ratios.

## 24. Explain Winsorizing and its purpose.
**Winsorizing:** Replaces outliers with nearest non-outliers.  
**Purpose:** Reduce outlier influence.

## 25. What is the midrange, and why is it rarely used?
**Midrange:** \( \frac{\text{Min} + \text{Max}}{2} \)  
**Drawback:** Sensitive to outliers.

## 26. What is Chebyshev’s inequality, and how is it used?
**Definition:** At least \(1 - \frac{1}{k^2}\) of data lies within k standard deviations from the mean, regardless of distribution.  
**Formula:** \( P(|X - \mu| \geq k\sigma) \leq \frac{1}{k^2} \)  
**Example:** For \(k=2\), at least 75% lies within 2 SDs.

## 27. What is the Durbin-Watson statistic?
**Definition:** Test for autocorrelation in regression residuals.  
**Range:** 0 to 4.  
**Use:** 2 = no autocorrelation, <2 = positive, >2 = negative autocorrelation.

## 28. What is the difference between sample size and standard error?
**Sample Size (n):** Number of observations.  
**Standard Error (SE):** \( SE = \frac{\sigma}{\sqrt{n}} \)  
**Example:** If \( \sigma = 10, n = 100 \Rightarrow SE = 1 \)

## 29. What is the Gini coefficient, and how is it calculated?
**Definition:** Measures inequality in a distribution.  
**Range:** 0 (equality) to 1 (inequality).  
**Formula:** \( G = \frac{\sum_{i=1}^{n}\sum_{j=1}^{n} |x_i - x_j|}{2n^2\mu} \)

## 30. What is entropy in the context of data distributions?
**Definition:** Measures uncertainty or disorder.  
**Formula:** \( H(X) = -\sum_{i=1}^{n} p(x_i) \log p(x_i) \)  
**Example:** Fair coin toss has \( H = 1 \) bit.

## 31. What is the Jaccard similarity coefficient?
**Definition:** Similarity between sets.  
**Formula:** \( J(A,B) = \frac{|A \cap B|}{|A \cup B|} \)  
**Example:** A = {1,2}, B = {2,3} \( \Rightarrow J = \frac{1}{3} \)

## 32. How do you calculate weighted averages?
**Formula:** \( \bar{x} = \frac{\sum w_i x_i}{\sum w_i} \)  
**Example:** (0.3 × 80 + 0.7 × 90) = 87

## 33. What is Spearman’s footrule?
**Definition:** Rank correlation using absolute rank differences.  
**Formula:** \( D = \sum_{i=1}^{n} |R_i - S_i| \)

## 34. What is Kendall’s tau?
**Definition:** Measures ordinal association.  
**Formula:** \( \tau = \frac{2(C - D)}{n(n-1)} \)  
**Range:** −1 to 1

## 35. What is Cronbach’s alpha?
**Definition:** Measures internal consistency.  
**Formula:** \( \alpha = \frac{k}{k - 1} \left(1 - \frac{\sum \sigma^2_i}{\sigma_X^2}\right) \)  
**Threshold:** \( \alpha > 0.7 \) is acceptable

## 36. What is item response theory (IRT)?
**Definition:** Models relationship between latent traits and responses.  
**Use:** Standardized testing.

## 37. What is principal component analysis (PCA)?
**Definition:** Reduces dimensionality via orthogonal transformation.  
**Steps:** Standardize, covariance, eigenvectors.  
**Use:** Reduce 10D to 2D.

## 38. What is factor analysis?
**Definition:** Identifies latent factors in variable correlations.  
**Example:** Satisfaction factors from survey data.

## 39. What is canonical correlation?
**Definition:** Correlation between two variable sets.  
**Example:** Health (BMI, BP) vs. Lifestyle (diet, exercise).

## 40. What is multiple correspondence analysis?
**Definition:** Visualizes associations in categorical variables.

## 41. What is t-distributed stochastic neighbor embedding (t-SNE)?
**Definition:** Visualizes high-dimensional data in 2D/3D.  
**Use:** Clusters, local structures (e.g., gene expression).

## 42. What is multidimensional scaling (MDS)?
**Definition:** Represents pairwise distances in lower dimensions.  
**Example:** Customer similarity mapping.

## 43. What is cluster analysis?
**Definition:** Groups similar data points.  
**Methods:** K-means (minimize variance), Hierarchical (dendrogram).

## 44. What is discriminant analysis?
**Definition:** Classifies into predefined groups.  
**Types:** LDA (linear), QDA (non-linear).

## 45. What is survival analysis?
**Definition:** Analyzes time-to-event data.  
**Key Metric:** \( S(t) = P(T > t) \)

## 46. What is time-to-event data?
**Definition:** Measures time until an event occurs.  
**Example:** Time to churn.

## 47. What is the hazard function?
**Definition:** Instantaneous risk given survival until \( t \).  
**Formula:** \( h(t) = \lim_{\Delta t \to 0} \frac{P(t \leq T < t + \Delta t \mid T \geq t)}{\Delta t} \)

## 48. What is censoring in survival analysis?
**Definition:** Event time is incomplete.  
**Types:** Right (not observed), Left (pre-observation).

## 49. What is the Kaplan-Meier estimator?
**Definition:** Estimates survival function non-parametrically.  
**Formula:** \( S(t) = \prod_{t_i \leq t} \left(1 - \frac{d_i}{n_i}\right) \)

## 50. What is the Cox proportional hazards model?
**Definition:** Regression for survival data.  
**Formula:** \( h(t) = h_0(t) \exp(\beta_1 X_1 + \ldots + \beta_p X_p) \)

