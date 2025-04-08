# Descriptive Statistics Questions and Answers

## 1. What is the difference between mean, median, and mode?
**Definition**:
- **Mean**: The average of all values.
- **Median**: The middle value in an ordered dataset.
- **Mode**: The most frequently occurring value.

**Formulas**:
- Mean: x̄ = ∑xᵢ / n
- Median: Middle value (or average of two middle values if n is even).
- Mode: Value with the highest frequency.

**Example**:
- For [2,3,3,5,7]: Mean = 4, Median = 3, Mode = 3

## 2. How do outliers affect the mean and median?
**Definition**:  
Outliers are extreme values that deviate significantly from other observations.

**Effect**:
- **Mean**: Sensitive to outliers (pulled toward extreme values).
- **Median**: Robust to outliers.

**Example**:
- For [1,2,3,4,100]: Mean = 22, Median = 3

## 3. What is the formula for calculating variance?
**Definition**:  
Variance measures the spread of data around the mean.

**Formulas**:
- Population variance: σ² = ∑(xᵢ−μ)² / N
- Sample variance: s² = ∑(xᵢ−x̄)² / (n−1)

**Example**:
- For [1,2,3,4,5], sample variance = 2.5

## 4. What does a standard deviation of zero indicate?
**Definition**:  
Standard deviation measures the average distance of data points from the mean.

**Interpretation**:
- If σ = 0, all values in the dataset are identical.

**Example**:
- Dataset [5,5,5] has σ = 0

## 5. Explain the interquartile range (IQR) and its use.
**Definition**:  
IQR is the range between the first quartile (Q1) and third quartile (Q3).

**Formula**:
- IQR = Q3 − Q1

**Use**:
- Identifies outliers and summarizes spread.

**Example**:
- For [1,3,5,7,9], IQR = 4

## 6. What is skewness? Describe left-skewed and right-skewed distributions.
**Definition**:  
Skewness is the asymmetry in the data distribution.

**Types**:
- **Left-skewed**: Tail on the left (mean < median).
- **Right-skewed**: Tail on the right (mean > median).

**Example**:
- Income data is typically right-skewed.

...

## 50. What is the Cox proportional hazards model?
**Definition**:  
A regression model for survival data.

**Formula**:  
h(t) = h₀(t)exp(β₁X₁ + ... + βₚXₚ)

- h₀(t): Baseline hazard
- β: Coefficients for predictors