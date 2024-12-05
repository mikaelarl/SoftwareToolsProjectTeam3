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

<img width="1042" alt="Income Distribution (Counties)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/countiesincomedist.png">
<img width="1042" alt="Income Distribution (Cities)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/citiesincomedist.png">
<img width="1042" alt="Income Distribution (Zip Codes)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/zipincomedist.png">

Let's examine the distribution of income for the highest level of geographic specificity, the zip-code level. 
<p align = "center">
<img width="800" alt="zipincomedist" src="https://github.com/user-attachments/assets/adcd88b5-20fb-4be0-8ec0-431b6331eef8"/>
</p>

As the captured by the histogram above, which displays a nearly bell-shaped distribution, median income seems to be fairly normal at the zip-code level. Further, the center of this distribution appears to lie around $30,000 to $33,000 per year. Note that there are some extreme values on both the high and low ends of the distribution, as is often characteristic of a normal bell-curve. 

Also examine the distribution of income for the next highest level of graphic specificity, the city level. 
<p align = "center">
<img width="800" alt="citiesincomedist" src="https://github.com/user-attachments/assets/b25fd30e-2190-43a3-a8f3-509829e004d6"/>
</p>

This histogram, which capture the distribution of median income at the city level, points to a slightly right-skewed distribution. With a right-, or positively- skewed distribution, most of the data lies at the lower end of the distribution, with some extreme values on the high-end of the distribution. For this type of distribution, the mean is often greater than the median, since the mean is sensitive to these extreme values. 

Next, let's examine the geographical distribution of both income and liquor sales ($) across the state of Iowa. Dashboards displaying the these geographical distributions at the zip-code, city, and county levels can be found below:

<img width="1042" alt="Maps Dashboard (Counties)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/countiesmapsdash.png">
<img width="1042" alt="Maps Dashboard (Cities)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/citiesmapsdash.png">
<img width="1042" alt="Maps Dashboard (Zip Codes)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/zipmapsdash.png">

Let's take a closer look at the geographical distribution of both income and liquor sales ($) in Iowa at the county level.
<p align = "center">
<img width="900" alt="" src="https://github.com/user-attachments/assets/1d95e265-5326-43f0-b49f-86476612e2fe"/>
</p>

Based on the stepped color encoding utilized within these two map visualizations, it appears as though there is a broad (though imperfect) relationship between median income and liquor sales for Iowa counties. Namely, regions with higher levels of income seem to also have higher annual liquor sales, per examination of the above dashboard (an interactive version of which can be found on the Tableau Public page linked at the beginning of this report). For example, Polk County, for which median income is relatively high, has particularly high annual liquor sales. However, this relationship is imperfect: Dallas County, which is in the highest income category, is actually in the lowest category for annual liquor sales, per the data visualization's stepped coloring. Nonetheless, it does seem that income and liquor sales do tend to adhere to a similar overall geographical pattern across the state of Iowa: low-income regions seem to generally exhibit lower liquor sales than high-income regions. 


Having established these general geopgraphical trends, let us examine the potential impact of income on liquor sales a bit more closely. Dashboards capturing the relationship between income and liquor sales at the county, city, and zip-code levels can be accessed below:

<img width="1042" alt="Income-Sales Dashboard (Counties)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/countiesincome-salesdash.png">
<img width="1042" alt="Income-Sales Dashboard (Cities)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/citiesincome-salesdash.png">
<img width="1042" alt="Income-Sales Dashboard (Zip Codes)" src = "https://github.com/mikaelarl/SoftwareToolsProjectTeam3/tree/main/zipincome-salesdash.png">

First consider the county-level dashboard: 

<p align = "center">
<img width="1221" alt="" src="https://github.com/user-attachments/assets/fa788713-8ef5-4f56-8952-24fae8bcb525"/>
</p>

The two side-by-side bar charts at the top of the dashboard capture the sales by liquor category, measured in both US$ and liters. Sales, measured both in US$ and liters, are highest by far for the whiskey and vodka categories. The liquor category with the third-highest sales performance is rum, both by dollar and liter measures. Amaretto has the lowest sales, both by dollar and liter measures. 

The two side-by-side scatter diagrams at the bottom of the dashboard capture the relationship between median income and dollar liquor sales. The scatter plot on the left displays this relationship in terms of total annual liquor sales, while the scatter plot on the right displays this relationship in per-capita terms. This per-capita visualization is important for the current analysis, as it adjusts for broad differences in population density across different geographical locations of Iowa. The bottom scatter diagram on the left generally affirms the positive relationship between median income and liquor sales observed perviously using heatmap visualizations. Further, notice that the linear trendline on the left scatterplot displays a positive slope. However, this positive relationship does not seem to be uniform across the income distribution: there are some very high levels of liquor sales at the middle-to-high end of the income distribution (approximately $35,000), which taper off at the high end of the income distribution. In other words, annual liquor sales seem to increase with median income until a certain income threshold (approximately $35,000), after which liquor sales drop starkly. This behavior of liquor sales relative to income (positive relationship, which tapers off after a threshold point), seems to hold in the right-hand scatter diagram, which captures liquor sales in per-capita terms.

It may also be useful to consider whether or not these trends persist across different levels of geographic specificity. Hence, we will now consider the zip-code-level dashboard capturing the relationship between income and liquor sales:

<p align = center>
<img width="1217" alt="zipincome-salesdash" src="https://github.com/user-attachments/assets/060a44d4-6798-447f-a2e2-51a8c52f0ebf"/>
</p>

As with the county-level dashboard, the two side-by-side bar charts at the top of the dashboard capture the sales by liquor category, measured in both US$ and liters. The top three sales performers and bottom sales performer are consistent between the county- and zip-code levels: the top three sales performers (in order) are whiskey, vodka, and rum, and the bottom sales performer is amaretto. As was the case at the county-level, these rankings are consistent across sales measures (dollars and liters). 

Discussion of the two scatter plots at the bottom of the dashboard, in comparison to the scatterplots displayed in the county-level dashboard, is perhaps more interesting. Unlike at the county-level, the linear trend line in the lefthand scatter diagram has a positive slope, suggesting that there is a negative relationship between median income and annual liquor sales, as measured in US$. In other words, the zip-code level data suggests, generally, that as median income increases, annual liquor sales decrease. This negative relationship is further affirmed by the right-hand scatter diagram, which displays the relationship between income and liquor sales in per-capita terms. 

Hence, while at the broadest level of geographical specificity within the dataset, there seems to be a positive relationship between income and liquor sales, this relationship does not neccessary hold as the data is deaggregated into city- and zip-code- levels of specificity. 

DISCUSS: WHY MIGHT THIS BE? POSITIVE AT COUNTY-LEVEL BUT NEGATIVE AT ZIP-CODE LEVEL? - IMPLICATIONS FOR ANALYSIS? - could mean that taxes should be county-level specific - counties with higher income have higher alcohol excise taxes

DISCUSS THE ADVANTAGES AND CHALLENGES OF PERFORMING ANALYSIS IN YOUR CHOSEN SOFTWARE TOOL

___

When looking at the merged dataset detailing income and alcohol consumption on the zip code level, it appears that most of the data reflects a relatively low amount of alcohol sales for Iowa residents residing in zip codes with an average income less than $20,000 and over $35,000. Those making incomes between $20,000 and $35,000 have higher alcohol sales volume per capita relative to residents of other zip codes with differing average income, and that contrast is heightened even further when considering alcohol sales in dollars per capita. The overwhelming majority of the data set is clustered towards low consumption of alcohol on a volume and dollars level, however there are a series of outliers for zip codes with an average income of $20,000-$35,000 as previously mentioned. Certain zip codes are not all that surprising, specifically zip codes 52401 and 50314 which represent the large cities Cedar Rapids and Des Moines respectively. Other zip codes such as 50033 (Madison County) and 51101 (Sioux City) also deviate from the norm of the dataset in having extremely high levels of spending on alcohol relative to their average salary, although part of this disparity might be attributable to their low population size. 


## 4. Conclusion


## 5. Policy Recommendation

