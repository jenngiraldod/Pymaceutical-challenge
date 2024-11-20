# Pymaceuticals Inc.
---
This is Jennifer Giraldo with my analysis
**Initial Setup and Data Loading**
The script imports essential libraries like matplotlib, pandas, and scipy.stats. Two datasets, Mouse_metadata.csv and Study_results.csv, are merged into a single DataFrame.

**Data Exploration**
The merged data is displayed for initial inspection. The script calculates the number of unique mice in the dataset.

**Data Cleaning**
Duplicate entries are identified based on Mouse ID and Timepoint. A clean dataset is created by removing rows corresponding to duplicate Mouse ID.

**Verification**
The number of unique mice in the cleaned dataset is rechecked.

***ANALYSIS***

**Mean and Median**
Useful for identifying which drug regimens result in the largest or smallest average tumor volumes.

**Variance and Standard Deviation**
Highlight the consistency of the effects of each drug regimen (e.g., high variability indicates inconsistent results).

**SEM**
Reflects the precision of the mean tumor volume estimates for each drug.

**Impact**
This analysis provides a clear overview of the performance and reliability of each drug regimen. The metrics are essential for identifying the most effective treatments and for planning further statistical tests.

## Analysis
The bar plot highlights how many data points (mouse timepoints) were recorded for each drug regimen. This provides an indication of the dataset's balance, showing whether all drug regimens are equally represented or if certain regimens have significantly more observations.

**Uneven Representation**
If some drug regimens have far fewer observations, it could affect the reliability of statistical analyses, as smaller sample sizes are more prone to variability. Over-represented regimens may dominate overall trends in the dataset.

**Impact on Analysis**
Drug regimens with more timepoints are likely to have more robust statistical measures (mean, variance, etc.).
Regimens with fewer observations may require further scrutiny, and results should be interpreted with caution.

finally, this plot is an effective way to assess the dataset's structure and ensure appropriate representation of all experimental groups.

# Analysis

**Gender Distribution**

The pie plot provides a visual representation of the balance between female and male mice in the study. The autopct parameter labels each section with the percentage of the total, offering a clear understanding of the proportions.

**Balance of Groups**

A near-equal distribution of male and female mice indicates that the study is well-balanced concerning sex. This is important to avoid gender bias in the results. An imbalance (one gender dominating the dataset) could skew findings and make them less generalizable.

**Impact on Analysis**

If the proportions are roughly equal, gender is unlikely to be a confounding factor. If there’s a significant imbalance, it might necessitate additional analyses to determine whether sex has an impact on the observed outcomes.

**Utility**

This visualization is useful for quickly assessing whether gender distribution in the study is appropriate for robust and unbiased conclusions.

# Analysis

**Central Tendency and Variability**

The box represents the interquartile range (IQR), with the line inside indicating the median tumor volume for each treatment group. This allows for quick comparisons of central tendencies (medians) across treatment groups.

**Spread and Consistency**

The length of the box and whiskers indicates variability. Narrow boxes suggest consistent results within the treatment group. Wider boxes or longer whiskers reflect greater variability in tumor volumes.

**Outliers**

The red markers highlight outliers, which are data points that fall outside the expected range (1.5 times the IQR above or below). Outliers may represent extreme responses or measurement errors and warrant further investigation.

**Treatment Comparisons**

Groups with lower median tumor volumes suggest better efficacy of the treatment in reducing tumors. Overlapping distributions indicate that differences between some treatments may not be statistically significant, requiring additional testing.

**Impact on Findings**

Treatments with low tumor volumes and tight variability (no outliers) can be identified as potentially more effective and consistent. Groups with high medians or large variability may indicate less effective treatments or inconsistent results.

# Analysis

**Trend Over Time**

The plot likely shows a decreasing trend in tumor volume over time, indicating the effectiveness of Capomulin in reducing the tumor size for this mouse. Any irregularities (e.g., spikes or plateaus) could reflect biological variability or measurement inconsistencies.

**Individualized Response**

This single-mouse analysis highlights how tumor volume responds to Capomulin treatment over time. While informative, it is an isolated case and should not be generalized without analyzing more mice.

**Impact on Analysis**

The consistent decrease in tumor volume, if observed, would support the efficacy of Capomulin for this particular case. The data offers a foundation for exploring trends across other mice treated with Capomulin, helping assess overall treatment effectiveness.

# Analysis

**Correlation Coefficient**

The calculated Pearson correlation coefficient is 0.84, indicating a strong positive correlation. This suggests that as the weight of the mouse increases, the average tumor volume also tends to increase. The correlation value is close to 1, showing a strong linear relationship between the two variables.

**Linear Regression Model**

The linear regression equation models the relationship between weight and tumor volume:

![image.png](attachment:cab32e82-0e3c-48ba-ba9f-6efe724daf72.png)

Where:

𝑦=is the predicted tumor volume.

𝑚 (slope)=quantifies how much the tumor volume increases per unit of weight.

𝑏(intercept)=represents the expected tumor volume when weight is zero.

The regression line plotted in orange visually represents this relationship.

**Scatter Plot**

The scatter plot shows individual data points, highlighting the observed variability in the relationship. The tight clustering around the regression line reinforces the strong positive correlation.

**Impact on Analysis**

The relationship between mouse weight and tumor volume may suggest that weight is a contributing factor to tumor growth or treatment response. It could also imply that heavier mice tend to develop larger tumors, which may need further biological investigation.
