# Statistics Cheat Sheet

This document provides concise explanations and formulas for key statistical concepts.

---

## 1. Difference Between Mean, Median, and Mode
**Mean**: Average of all values.  
**Median**: Middle value in an ordered dataset.  
**Mode**: Most frequently occurring value.

**Formulas:**  
- Mean: \( \bar{x} = \frac{\sum x_i}{n} \)  
- Median: Middle value (or average of two middle values if \( n \) is even)  
- Mode: Value with the highest frequency

**Example:** [2, 3, 3, 5, 7] → Mean = 4, Median = 3, Mode = 3

---

## 2–25. [Omitted for brevity – Assume content exists here.]

---

## 26. What is Chebyshev’s inequality, and how is it used?
**Definition**: A theorem stating that at least \(1 - \frac{1}{k^2}\) of data lies within k standard deviations from the mean, regardless of the distribution.  
**Formula**: \(P(|X−\mu| ≥ k\sigma) ≤ \frac{1}{k^2}\)  
**Example**: For k=2, at least \(1−\frac{1}{4} = 75\%\) of data lies within 2 SDs of the mean.

## 27. What is the Durbin-Watson statistic?
**Definition**: A test for autocorrelation in regression residuals.  
**Range**: 0 to 4.  
- 2: No autocorrelation.  
- <2: Positive autocorrelation.  
- >2: Negative autocorrelation.  
**Use**: Detect serial correlation in time series data.

## 28. What is the difference between sample size and standard error?
**Sample Size (n)**: Number of observations.  
**Standard Error (SE)**: \(SE = \frac{\sigma}{\sqrt{n}}\)  
**Relationship**: Larger n reduces SE, increasing precision.  
**Example**: If \(\sigma = 10\) and \(n = 100\), then \(SE = 1\).

## 29. What is the Gini coefficient, and how is it calculated?
**Definition**: Measures inequality in a distribution.  
**Formula**: \(G = \frac{\sum_{i=1}^{n}\sum_{j=1}^{n} |x_i - x_j|}{2n^2\mu}\)  
**Range**: 0 (Perfect equality) to 1 (Maximum inequality).  
**Example**: Used to assess income inequality.

## 30. What is entropy in the context of data distributions?
**Definition**: Measures uncertainty or disorder in a distribution.  
**Formula**: \(H(X) = −\sum_{i=1}^{n} p(x_i) \log p(x_i)\)  
**Example**: A fair coin toss has entropy \(H = 1\) bit.

## 31. What is the Jaccard similarity coefficient?
**Definition**: Measures similarity between two sets.  
**Formula**: \(J(A,B) = \frac{|A \cap B|}{|A \cup B|}\)  
**Example**: For sets A={1,2} and B={2,3}, \(J = \frac{1}{3}\).

## 32. How do you calculate weighted averages?
**Formula**: \(\bar{x} = \frac{\sum w_i x_i}{\sum w_i}\)  
**Example**: Course grade = \((0.3×80)+(0.7×90) = 87\)

## 33. What is Spearman’s footrule?
**Definition**: Measures rank correlation by summing absolute differences in ranks.  
**Formula**: \(D = \sum_{i=1}^{n} |R_i - S_i|\)  
**Use**: Less sensitive to outliers than Pearson’s correlation.

## 34. What is Kendall’s tau?
**Definition**: Measures ordinal association between two variables.  
**Formula**: \(\tau = \frac{2(C−D)}{n(n−1)}\)  
- C: Concordant pairs.  
- D: Discordant pairs.  
**Range**: −1 to 1.

## 35. What is Cronbach’s alpha?
**Definition**: Measures internal consistency of a test.  
**Formula**: \(\alpha = \frac{k}{k-1} \left(1 - \frac{\sum \sigma^2_i}{\sigma^2_X} \right)\)  
- k: Number of items.  
- \(\sigma^2\): Variance of item scores.  
**Threshold**: \(\alpha > 0.7\) is acceptable.

## 36. What is item response theory (IRT)?
**Definition**: A framework to model the relationship between latent traits (e.g., ability) and observed responses.  
**Example**: Used in standardized testing to score examinees.

## 37. What is principal component analysis (PCA)?
**Definition**: Reduces dimensionality by transforming data into orthogonal components.  
**Steps**:  
- Standardize data.  
- Compute covariance matrix.  
- Extract eigenvectors (principal components).  
**Example**: Compress 10 variables into 2 PCs.

## 38. What is factor analysis?
**Definition**: Identifies latent factors that explain correlations among observed variables.  
**Example**: Grouping survey questions into underlying traits (e.g., "satisfaction").

## 39. What is canonical correlation?
**Definition**: Measures the correlation between two sets of variables.  
**Example**: Relationship between health metrics (e.g., BMI, BP) and lifestyle factors (e.g., diet, exercise).

## 40. What is multiple correspondence analysis?
**Definition**: Extends correspondence analysis to categorical variables.  
**Use**: Visualizes associations between categories.

## 41. What is t-distributed stochastic neighbor embedding (t-SNE)?
**Definition**: A tool to visualize high-dimensional data in 2D/3D.  
**Key Feature**: Preserves local structures (clusters).  
**Example**: Visualizing clusters in gene expression data.

## 42. What is multidimensional scaling (MDS)?
**Definition**: Represents pairwise distances between objects in lower dimensions.  
**Example**: Mapping customer similarity based on purchasing behavior.

## 43. What is cluster analysis?
**Definition**: Groups similar data points into clusters.  
**Methods**:  
- K-means: Minimizes within-cluster variance.  
- Hierarchical: Builds a dendrogram.

## 44. What is discriminant analysis?
**Definition**: Classifies data into predefined groups.  
**Types**:  
- Linear (LDA): Assumes normality.  
- Quadratic (QDA): Allows non-linear boundaries.

## 45. What is survival analysis?
**Definition**: Analyzes time-to-event data (e.g., death, failure).  
**Key Metric**: Survival function \(S(t)=P(T>t)\).

## 46. What is time-to-event data?
**Definition**: Data where the outcome is the time until an event occurs.  
**Example**: Time until a customer churns.

## 47. What is the hazard function?
**Definition**: The instantaneous risk of an event at time t, given survival until t.  
**Formula**: \(h(t)=\lim_{\Delta t→0} \frac{P(t≤T<t+\Delta t | T≥t)}{\Delta t}\)

## 48. What is censoring in survival analysis?
**Definition**: When the event is not observed for some subjects.  
**Types**:  
- Right-censoring: Event not observed (e.g., study ends).  
- Left-censoring: Event occurred before observation.

## 49. What is the Kaplan-Meier estimator?
**Definition**: Estimates the survival function non-parametrically.  
**Formula**: \(S(t)= \prod_{t_i ≤ t}(1−\frac{d_i}{n_i})\)  
- \(d_i\): Events at time \(t_i\).  
- \(n_i\): Subjects at risk at \(t_i\).

## 50. What is the Cox proportional hazards model?
**Definition**: A regression model for survival data.  
**Formula**: \(h(t)=h_0(t)\exp(\beta_1X_1 +⋯+\beta_pX_p)\)  
- \(h_0(t)\): Baseline hazard.  
- \(\beta\): Coefficients for predictors.

