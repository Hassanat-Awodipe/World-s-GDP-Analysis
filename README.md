# World's GDP Exploration
## by Hassanat Awodipe


## Dataset

The dataset was gotten from [kaggle](https://www.kaggle.com/datasets/truecue/worldsustainabilitydataset?select=WorldSustainabilityDataset.csv) and it was compiled from World bank. It contained two tables: **World Sustainability dataset** which contained the economic data of countries in the world from 2000 t0 2018 and the **Data dictionary** which described the features in the table.

The table initially contained a number of nulls values. For the important columns: GDP and Population, I dropped the null rows. For this reason, my analysis started from the year 2001 with 3,072 observations from 172 unique countries. This data cleaning process was done in MS Excel. The null values in the other numeric columns such as `exports`, `imports` were filled with the corresponding mean values.


## Summary of Findings

GDP had a fairly normal distribution after scaling its axis logarithmically. The features with null values(exports, imports, total natural resources, gross savings) had an abnormally tall bar which represented the nulls that were filled with mean values.

During the bivariate exploration, I found out that there was a rise and fall in the GDP from 2010 to 2018. So, I examined the correlation between GDP and its numeric features for those years to find its possible cause. There was a positive correlation between GDP and Population and a negative correlation between GDP and imports. Then, I further examined GDP and imports for each of the years involved but there was no conclusive insight.

A mulitvariate plot of GDP, Population and Imports for the years 2010-2018 showed that low imports was associated with high GDP and high population. This was also seen when imports and exports were plotted against income class. High income classes had their imports and exports to be equal whereas the other income classes had higher imports and lower exports.

Sub-Sahara Africa region had the highest count of observations while High Income Class occurred the most in the dataset. Even with these, more points of Sub Sahara Africa consistently showed up in Low income when Regions and Income Class were plotted against the numeric features. Eastern and Southern Asia had points scattered around all Income Classes. Europe and Northern America & Northern Africa and Western Asia always had noticeable points in the High Income and Upper middle income Class.   

The average GDP Per Capita was outrageously high for high income class compared to the other income classes for all 7 regions except Central and Southern Asia. 

Central and Southern Asia had no bar for high income class it but had the third-highest maximum GDP as seen in the violin plot of Regions vs GDP and Population. This suggests that at the time it had a high maximum GDP, the high income range had moved up.

## Key Insights for Presentation

For the presentation, I mainly focused on **GDP, population and income class**. I showed how the growth of population aligned with that of GDP. I tried to figure out the cause of the fall of GDP in 2015 but the features which were negatively correlated with GDP did not produce any valuable insight.

Thereafter, I introduced the categorical variables and showed their distribution with GDP and Population. Then, I engineered the **GDP per capita** feature to illustrate the effect of Population on GDP by regions and income class. 