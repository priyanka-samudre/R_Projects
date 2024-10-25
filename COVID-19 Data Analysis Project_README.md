# COVID-19 Data Analysis Project
## Project Overview
This project aims to analyze the COVID-19 dataset to uncover insights about mortality rates, particularly focusing on the relationship between age, gender, and death outcomes. The project explores whether age and gender significantly impact the likelihood of death due to COVID-19 using statistical analysis techniques.

## Objectives
Death Rate Calculation: Calculate the overall death rate from the dataset.

Age Analysis: Investigate whether older individuals are more likely to die from COVID-19.

Gender Analysis: Test the hypothesis that gender has no effect on mortality rate.

Statistical Significance: Conduct t-tests to determine if the differences between groups (age and gender) are statistically significant.

## Key Steps and Methodology
#### 1. Data Cleaning
The column related to death was cleaned up by creating a binary column (death_dummy) where 1 represents death and 0 represents survival.
#### 2. Overall Death Rate
The death rate was calculated as the ratio of the total number of deaths to the total number of records in the dataset.
#### 3. Age and Mortality
The mean age of those who died was compared to the mean age of those who survived.
A two-sided t-test was conducted to determine if the difference in age between the two groups (dead vs. alive) was statistically significant.
#### 4. Gender and Mortality
The death rates for men and women were calculated separately.
A two-sided t-test was conducted to evaluate whether the difference in death rates between men and women was statistically significant.
## Key Findings
#### 1. Death Rate
The overall death rate from the dataset is approximately 4.74%.
#### 2. Age and Mortality
The average age of those who died is 68.39 years, while the average age of survivors is 48.94 years.
The t-test returned a p-value close to zero, meaning the difference in age between the two groups is statistically significant. Older individuals are indeed more likely to die from COVID-19.
#### 3. Gender and Mortality
The death rate for men is 8.5%, while for women, it is 3.7%.
The t-test yielded a p-value of 0.002, indicating that the difference in death rates between men and women is also statistically significant. Men are more likely to die from COVID-19 than women, with a 99% confidence interval showing that men have between 0.8% to 8.8% higher chance of dying compared to women.
## Conclusion
The analysis confirms that both age and gender are statistically significant factors in COVID-19 mortality:

Older people are more likely to die from the disease.
Men have a higher mortality rate compared to women.
This information could be critical in shaping public health strategies, especially in targeting higher-risk groups with preventive measures.

Tools and Techniques Used
R Programming: For data cleaning, analysis, and statistical testing.
Libraries: Hmisc for data description, t.test for statistical testing.
Statistical Methods: T-tests for determining the significance of differences between groups.
