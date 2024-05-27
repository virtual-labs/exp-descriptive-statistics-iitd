<img src="images/Image 27-03-23 at 12.37 PM.jpg"/>
<img src="images/Image 27-03-23 at 12.37 PM (1).jpg"/>
<img src="images/Image 27-03-23 at 12.38 PM.jpg"/>
<img src="images/Image 27-03-23 at 12.39 PM.jpg"/>
<img src="images/Image 27-03-23 at 12.39 PM (1).jpg"/>
<img src="images/Image 27-03-23 at 12.40 PM.jpg"/>
<img src="images/Image 27-03-23 at 12.40 PM (1).jpg"/>
<img src="images/Image 27-03-23 at 12.43 PM.jpg"/>
<img src="images/Image 27-03-23 at 12.44 PM.jpg"/>
<img src="images/Image 27-03-23 at 12.41 PM.jpg"/> 
<img src="images/Image 27-03-23 at 12.42 PM.jpg"/>


# Covariance and Correlation Coefficient

## Covariance

**Covariance** is a measure of how much two random variables change together. If greater values of one variable mainly correspond with greater values of the other variable, and the same holds for lesser values, the covariance is positive. If greater values of one variable mainly correspond with lesser values of the other, the covariance is negative. 

### Mathematical Definition

For two random variables \(X\) and \(Y\), the covariance is defined as:

\[ \text{Cov}(X, Y) = \mathbb{E}[(X - \mu_X)(Y - \mu_Y)] \]

where:
- \(\mathbb{E}\) denotes the expectation.
- \(\mu_X = \mathbb{E}[X]\) is the mean of \(X\).
- \(\mu_Y = \mathbb{E}[Y]\) is the mean of \(Y\).

In a sample, the covariance between two variables \(X\) and \(Y\) can be estimated as:

\[ \text{Cov}(X, Y) = \frac{1}{n-1} \sum_{i=1}^n (X_i - \bar{X})(Y_i - \bar{Y}) \]

where:
- \(X_i\) and \(Y_i\) are the individual sample points.
- \(\bar{X}\) is the sample mean of \(X\).
- \(\bar{Y}\) is the sample mean of \(Y\).
- \(n\) is the number of data points.

### Interpretation

- **Positive covariance**: Indicates that as \(X\) increases, \(Y\) tends to increase.
- **Negative covariance**: Indicates that as \(X\) increases, \(Y\) tends to decrease.
- **Zero covariance**: Indicates no linear relationship between \(X\) and \(Y\).

## Correlation Coefficient

**Correlation coefficient** (specifically, Pearson's correlation coefficient) is a normalized measure of the strength and direction of the linear relationship between two variables. It is dimensionless and ranges from \(-1\) to \(1\).

### Mathematical Definition

The Pearson correlation coefficient \(r\) between two variables \(X\) and \(Y\) is defined as:

\[ r_{XY} = \frac{\text{Cov}(X, Y)}{\sigma_X \sigma_Y} \]

where:
- \(\text{Cov}(X, Y)\) is the covariance between \(X\) and \(Y\).
- \(\sigma_X\) is the standard deviation of \(X\).
- \(\sigma_Y\) is the standard deviation of \(Y\).

In a sample, it is calculated as:

\[ r_{XY} = \frac{\sum_{i=1}^n (X_i - \bar{X})(Y_i - \bar{Y})}{\sqrt{\sum_{i=1}^n (X_i - \bar{X})^2 \sum_{i=1}^n (Y_i - \bar{Y})^2}} \]

### Interpretation

- \( r = 1 \): Perfect positive linear relationship.
- \( 0 < r < 1 \): Positive linear relationship.
- \( r = 0 \): No linear relationship.
- \( -1 < r < 0 \): Negative linear relationship.
- \( r = -1 \): Perfect negative linear relationship.

## Properties

1. **Range**: The correlation coefficient always lies between \(-1\) and \(1\).
2. **Symmetry**: \( r_{XY} = r_{YX} \).
3. **Unit-free**: The correlation coefficient is dimensionless.

## Relation Between Covariance and Correlation

Covariance measures the degree to which two variables vary together, but its magnitude depends on the units of the variables. Correlation normalizes this measure, providing a dimensionless metric that can be easily interpreted.

## Summary

- **Covariance** quantifies the direction of the linear relationship between variables.
- **Correlation coefficient** quantifies both the direction and the strength of the linear relationship, normalized to a range between \(-1\) and \(1\).

Understanding these concepts is crucial in statistics and data analysis as they provide insights into the relationships between variables, which can inform decision-making and hypothesis testing.
