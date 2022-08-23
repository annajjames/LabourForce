## Introduction
Canada has been a land of immigrants since the 16th century, a trend that continues today. As of 2020 there are above 8 million immigrants with permenant residents living in Canada making up 21.5% of the total population.
Our dataset is from Ontario Provincial website and has the information on the labor force from March 2006 to November 2020 by age group, sex, education level, and immigrant years since landing in Canada/Ontario.

## Objective
To analyze:
- Time series, trend, seasonality, and autocorrelation for unemployment in different education levels and immigration groups (based on immigrant years since landing in Canada)
- Statistical significance using ANOVA test and 2-sample t-test for:
    - unemployment across different education levels for age greater than 25
    - unemployment across different immigration groups
    - unemployment between males and females for age greater than 25
The 3 categories of education levels are:
Level123: No degree, certificate, or diploma
Level45: Post-secondary certificate or diploma
Level67: University degree

## Key Findings
#### Unemployment across education levels for age>25 in Ontario
- Unemployment signals for all three education levels are periodic.
- Unemployment trends for education level123 and level45 has a gradual decrease after the 2009 recession. This means unemployments has been decreasing in these two levels.
<img width="825" alt="Trend_unemp1" src=“https://user-images.githubusercontent.com/58715002/186259163-6d9f0bb3-ff3a-4676-abe6-3118ba7aeff9.png">
                                                                                                                                                    
- Periodicity in unemployment levels in all three education levels may be attributed to the flow of immigrants, contract-based jobs.
- Autocorrelation plots for unemployment in level123 and level45 suggests 2 months of high unemployment followed with a month of low unemployment.
- For data before February 2020, unemployment averages between different education levels is statistically significant at 0.05.
- For data between February and November 2020, unemployment averages between different education levels is comparable and the probability of obtaining the same unemployment average between education levels is close to 44% making it not statistically significant at 0.05. In other words unemployment was similar in all levels from February to November 2020.
<img width="683" alt="unemp_boxplots" src="https://user-images.githubusercontent.com/58715002/186265532-607ac6d7-2c5b-45bc-b5be-082c2dba101b.png">
<img width="639" alt="unemp_bonftabs" src="https://user-images.githubusercontent.com/58715002/186266595-1c7fbc3e-4edb-4aa4-bf1a-951345d63079.png">
- Population for education level123 have been gradually decreasing in Ontario since 2006 whereas populations for level45 and level67 has been increasing. This can possibly mean that more people are choosing to complete their post-secondary certificate or diploma or university, or immigrants moving to Ontario in education level123 is decreasing, or population from level123 are moving out of Ontario to other provinces.
<img width="486" alt="unemp_pop" src="https://user-images.githubusercontent.com/58715002/186268890-ac5179c0-5b86-49a2-b7e0-ab590859d7b8.png">                                                                                                                                               

#### Unemployment between males and females for age>25 in Ontario
- At 0.86% the average unemployment difference between males and females in Ontario is less than 1% with more males unemployed than females. But at a significance level of 0.05 this difference is statistically significant.
- During covid the average unemployment difference between males and females reduced and was 0.13%. The probability of getting the same unemployment averages for males and females was greater than 93% making the difference not significant.

## Data Source
https://data.ontario.ca/dataset/labour-force-estimates-by-immigration
