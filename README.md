# EPI-and-Corruption

Loaded epi_countries dataset from epi Postgresql data base and cpi dataset from csv file. Created dataframes 
from each of them.
cpi dataframe contains list of countries, their Environment Performance Indices and various scores that indicate air health, water health, forestries, etc
epi dataframe contains countries and each country's Corruption Perceptions Index. The higher the index, the better that country handles corruption.

The goal was to find out if there is a correlation between CPI and EPI.

I used seaborn plots to make visualizations that help to see if there is a connection betweeen cpi and environment health categories.

When making the plots on cpi and epi we could infer that countries that handle corruption better have higher epi. However, when I made graphs on separate categories like cpi impact on forestry, the connection wasn't obvious. Since some countries with pretty low cpi had high index on forestry.

In order to find connections between corruption and environmental health one needs a more comprehensive dataset. I wish the dataset had some kind of corruption scores on each country's biggest industries. Various industries could directly lead to deforestation or water pollution and so on. I would like to gather more information on that.


I've used sklearn LinearRegression to train ML model on the data. The data was split into training and test data. The model was supposed to predict epi score on cpi score. The model seems to be underfitting, it performed poorly on the training data. The reason for poor performance could be because the model is too simple. In order to improve model's performance, we need to add more domain-specific input features.

I've used Tableau to create some visualizations in order to confirm or refute my observations above in regards of connection between CPI and EPI.

I've got similar results. In general we can infer - the higher the CPI, the higher the EPI is. It looks like there are less violations and environmental damage in the countries with better handle on corruption. However, as I mentioned above, there is a great ammount of countries with terrible CPI score and decent levels on various environmental metrics' health. We need more extensive data to be able to make valid assumptions.

My Tableau dashboard: https://prod-useast-a.online.tableau.com/#/site/anastasiyaayalacom/workbooks/874788?:origin=card_share_link
