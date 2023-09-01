## Problem Statement
We want to know if the unemployment rates between different groups (age > 25) during Covid lockdowns (from Feb 2020) is statistically significant or not.
1. Is the average unemployment between different education levels significant?
2. Is the average unemployment rate between males and females significant?

## Background
In 2020 Covid caused disruption in all aspects of human life.
We have data on the labor force of Ontario and Canada from March 2006 to November 2020 by age group, sex, education level, and immigrant years since landing in Canada.
This dataset is from Ontario Provincial website.
The 3 categories of education levels are:
Level123: No degree, certificate, or diploma
Level45: Post-secondary certificate or diploma
Level67: University degree

## Objective
1. Perform ANOVA test and Multi-comparison all pair test with Bonferroni correction for unemployment across different education levels (ages 25 - 64) for data before Feb 2020 and data during covid from Feb 2020 to Nov 2020.
2. Perform 2-sample t-test for unemployment between males and females for data before Feb 2020 and data during covid from Feb 2020 to Nov 2020.
3. Analyze the time series, trend, seasonality for unemployment in different education levels and immigration groups (based on immigrant years since landing in Canada).

## Key Findings
#### Unemployment across education levels in Ontario (for age>25 )
- For data before February 2020, the average unemployment between different education levels is different and statistically significant at 0.05.
- For data between February and November 2020, unemployment averages between different education levels is comparable and the probability of obtaining the same unemployment average between education levels is close to 44% making it not statistically significant at 0.05. In other words unemployment was similar in all levels from February to November 2020.
<img width="683" alt="unemp_boxplots" src="https://user-images.githubusercontent.com/58715002/186265532-607ac6d7-2c5b-45bc-b5be-082c2dba101b.png">
<img width="650" alt="unemp_bonftabs" src="https://user-images.githubusercontent.com/58715002/186266595-1c7fbc3e-4edb-4aa4-bf1a-951345d63079.png">
                                                                                                                                    
#### Unemployment between males and females in Ontario (for age>25 )
- The average unemployment difference between males and females in Ontario is less than 1% with more males unemployed than females. But this difference is statistically significant at a significance level of 0.05.
- During covid the average unemployment difference between males and females reduced and was 0.13%. The probability of getting the same unemployment averages for males and females was 93%. That is, during Covid lockdowns the unemployment rate between males and females is same and not statistically significant.
<img width="683" alt="MaleF_unemp" src="https://user-images.githubusercontent.com/58715002/186394251-050d96a0-70d5-4e08-b069-26c5f8ce8477.png">

