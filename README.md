# ADEC 7900 Software Tools Project - Team 3
#### Paul Gaski, Michael Pomer, Mikaela Renaud-Lowther, and Justin Nevins

## Important Deliverables 
### Project Report:
Our group project report, entitled "Project Report.rmd" can be located in the main branch. 

### Dashboards on Tableau Public:
Dashboards pertaining to our analysis can be accessed on Tableau Public at the following link: https://public.tableau.com/app/profile/mikaela.renaud.lowther/vizzes 

## Research Topic
### The Question: 
To what extent does an individual's income affect their consumption of alcohol in Iowa?
### The Decision-Maker and the Decision To-Be-Made:
Local policymakers evaluating the efficacy of alcohol excise taxes and determining future levels of these taxes
### The Data:
The current analysis will employ two main categories of data from two different data sources: data on the sale of liquors in Iowa from the Iowa Department of Revenue and data capturing Iowa's demographic and economic characteristics from the American Community Survey. Both of these sources record three levels of geographic specificity, providing data at the county-, city-, and zip-code- level. Key variables within the data (namely "income," "population," "sale.dollars," and "sale.volume") having been observed across different geographical levels will be an important asset for our analysis. 

## The 8 Major Tasks
1. Create a GitHub repository and establish best practices for team collaboration.
2. Analyze and visualize ACS data using Tableau and/or R.
3. Analyze and visualize aggregated sales data using Tableau and/or R.
4. Merge aggregated liquor sales data with ACS data per each geography (zipcodes, cities, counties). This will result in 3 data sets. If using Tableau, create 3 workbooks.
5. Visualize and identify patterns in liquor sales across geographies and ACS metrics using R and/or Tableau.
6. Submit draft of progress at Checkpoint 1 and Checkpoint 2.
7. Summarize your findings in a short video presentation.
8. Publish a detailed, well-formatted R-markdown report of your analytical story to your GitHub repository (see project instructions for details).

## Checkpoint 1 Progress
Our group has completed tasks 1 and 4. We have been working on tasks 2, 3, and 5 (analyzing and visualizing our data in order to identify relevant trends). We are finding using GitHub as a collaborative platform to be quite helpful for aiding our work as a group. It is also useful in tracking individual changes and progress. 

### Checkpoint 1 Individual Group Member Contributions: 

Mikaela: I have created a variety of visualizations for the county-level data, which can be located in the "Liquor Sales Counties.twb" Tableau workbook. I have also created an R-markdown file entitled "County-LevelRAnalysis.rmd," within which I constructed numerous linear models in order to estimate the causal effect of income on average dollar sales. 

Paul: I have merged the aggregated liquor sales data with ACS data per each geography (zip codes, cities, counties) and uploaded these 3 new data sets using Tableau as 3 individual workbooks to Github, to help with completing additional major project tasks.

Mick: I created a heat map in Tableau that illustrates how the income of different zip codes differ throughout Iowa. I also
wrote an analysis to make conclusions and observations pertaining to the heat map, specifically relating to income "hot spots" and the significance of Iowa's geography when considering income and alcohol consumption.

## Checkpoint 2 Progress
Our group has continued to work on tasks 2, 3, and 5. We have also started working on task 8. We have initialized an R Markdown file for our Project Report, added it to the Team_3Checkpoint_2.0 Branch, and began working on the early sections of the report. Collaborating on GitHub countinues to be a helpful way to track the individual contributions of different team members and keep all of our up-to-date files in one place. 

### Checkpoint 2 Individual Group Member Contributions

Mikaela: I created similar visualizations for the city- and zip-code-level data as I created for the county-level data. These visualizations can be located in the "Liquor Sales Cities.twb" and "Liquor Sales Zip-Codes.twb" Tableau worksheets, respectively, within the Team_3Checkpoint_2.0 Branch. I also created a new measure, "sale.dollars.percap," within each of the 3 Tableau worksheets. I then created a scatter diagram, for each level of geographic specificity, plotting per capita dollar sales against income. I also created an R Markdown file for our project Report and uploaded it to the Team_3Checkpoint_2.0 Branch. Within this R Markdown file, entitled "Project Report.rmd," I began working on the "Introduction" and "Data Summary" sections of the Report. 

Paul: I have focused on Cities based analysis for this Checkpoint, as County and Zip Code analysis are being worked on by other group members. I have built out a Tableau file with multiple Dashboards and a Story focused on visualizing Iowa Cities Income and Liquor Consumption behaviors.

Justin: For this Checkpoint, I have focused on R level analysis where I merged ACS and liquor sales data for both zip codes and cities. From there, I created visualizations of certain summary statistics to begin to understand the relationships between variables. I addittionally created numerous correlations and correlation heatmaps to show the effect that certain variables had on others. Finally I developed in depth regression models that incorporate important demographics that explain statistical significance towards liquor sales. These models have the additional capability to predict liquor sales based on these particular demographics. I include the R markdown files as well as the html outputs that show these visualizations. 

Mick: Analyzed merged dataset for alcohol consumption pertaining to zip codes in the report file. Singled out particular 
data points that were deemed to be excursions and made conclusions about basic trends related to the central research question. 
