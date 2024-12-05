# ADEC 7900 Software Tools Project - Team 3
#### Paul Gaski, Michael Pomer, Mikaela Renaud-Lowther, and Justin Nevins

### Dashboards on Tableau Public:
Dashboards pertaining to our analysis can be accessed on Tableau Public at the following link: https://public.tableau.com/app/profile/mikaela.renaud.lowther/vizzes 


## 1. Introduction

Broadly, the current analysis intends to investigate the relationship between an individual's income and their purchase of liquor. The nature of this potential relationship is of key importance for policymakers who determine the level of different taxes for a specific geographic area. One type of tax in particular, the alcohol excise tax, is especially relevant to this discussion because it is a selective tax placed on the purchase of alcohol. While the alcohol producer pays this tax at the level of the wholesale transaction, the burden of the tax is in practice placed on the consumer, who is forced to pay a higher retail value for the alcohol. Hence, alcohol excise taxes are often implemented in order to disincentivise the purchase and consumption of alcohol. 

With these dynamics in mind, the current analysis will examine the question, *To what extent does an individual's income affect their purchase (and assumed consumption) of alcohol in Iowa?*

The decision-maker in our analysis is a group of local policymakers evaluating the potential efficacy of alcohol excise taxes. The decision-to-be-made is the optimal level(s) and distribution of these excise taxes across the state of Iowa. Setting tax levels can be a delicate art for policymakers, as they must consider various goals, including both business revenue and social outcomes. The decisions of policymakers not only influence Iowa residents, but can also serve as an example (or lesson) for policymakers across the country. 


## 2. Data Summary

The current analysis combines data from two sources, both of which cover three levels of geographic specificity (county level, city level, and zip-code level). The first source is the Iowa Department of Revenue, which provides data on the sales of liquors in Iowa. More specifically, this data captures the total sales in both dollars and liters across various liquor categories in Iowa from 2012 to 2016. The second source is the American Community Survey, which provides demographic and economic data for the state of Iowa. More specifically, this data captures total population, income, unemployment, education, and race across the state of Iowa from 2012 to 2016. In combination, these two data sets provide data on both income and liquor sales at the county-, city-, and zip-code levels, which will serve as the basis for our analysis. 

ADD DESCRIPTIVE STATISTICS AS APPLICABLE 


## 3. Data Analytics

It might first be helpful to examine the distribution of our main causal variable of interest, income. Histograms displaying the distribution of median income at the zip-code, city, and county levels can be found below: 

<img width="1042" alt="zipincomedist" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/countiesincomedist.png">


When looking at the merged dataset detailing income and alcohol consumption on the zip code level, it appears that most of the data reflects a relatively low amount of alcohol sales for Iowa residents residing in zip codes with an average income less than $20,000 and over $35,000. Those making incomes between $20,000 and $35,000 have higher alcohol sales volume per capita relative to residents of other zip codes with differing average income, and that contrast is heightened even further when considering alcohol sales in dollars per capita. The overwhelming majority of the data set is clustered towards low consumption of alcohol on a volume and dollars level, however there are a series of outliers for zip codes with an average income of $20,000-$35,000 as previously mentioned. Certain zip codes are not all that surprising, specifically zip codes 52401 and 50314 which represent the large cities Cedar Rapids and Des Moines respectively. Other zip codes such as 50033 (Madison County) and 51101 (Sioux City) also deviate from the norm of the dataset in having extremely high levels of spending on alcohol relative to their average salary, although part of this disparity might be attributable to their low population size. 


## 4. Conclusion


## 5. Policy Recommendation

