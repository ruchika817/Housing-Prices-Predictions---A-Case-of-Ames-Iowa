
## Problem Statement
What are the most important factors that determine house prices - The case of Ames, Iowa.

I am a researcher hired by a professor who is writing a paper on what makes housing prices go up. This is an important question for homeowners as well as financial institutions who predict house prices based on data.

With this [dataset on houses](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt) from Ames, Iowa, I run regression models to figure out the best model to predict house prices.


# Executive summary
 As a data scientist hired by a professor writing a paper about what determines a house price in small town USA, I was given the task of running regression analysis on a dataset from Ames, Iowa. Ames is a University town in Central Iowa with a population of 66,478 as of the 2017 census. It is home to the Iowa State University. Half of the population of the town is made up of students of this University. As a result, the houses on rent in Ames are a large proportion of the real estate properties in town.

The [Ames Dataset](https://www.kaggle.com/c/dsi-us-10-project-2-regression-challenge/data) is a dataset of all features of houses sold in Ames, IA between 2006-10. The purpose of this project is to determine the factors that lead to higher sale prices and what makes a house sell.

There are 80 columns of variables in the dataset. Out of these there are 20 continuous variables, 23 nominal, 23 ordinal and 13 discrete variables. These all describe every aspect of houses.[Data Description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt).

Besides this data I created a few variables
Bsmt Bathroom = Basement Full Bathroom + 0.5 * Half Bathrooms.
Total SF = Above ground SF + Basement SF

There were a lot of issues with the dataset. There were a number of columns with a large number of null values. They had to be fixed. There were a lot of ordinal and nominal non numerical data with values as NA. These were not missing values but a separate category showing that that particular characteristic was not present in that house. These values had to be given a value. And the ordinal variables had to be given weight according to their ranking. And there were also categorical variable that were one hot encoded into dummy variables. By the end of this I had 157 columns and 2050 rows.


# Conclusions
There were some interesting findings from my analysis. As expected, the size of the house and the overall condition of the house had the maximum impact on house prices. These two variables alone accounted for 77% of the variability of the house price. There were some neighborhoods that seemed more desirable and had higher prices. The unexpected findings in my analysis was that the Basement exposure and the Finished basement variable were very significant. Realizing that Ames, Iowa is in tornado country explains that finding. Also the neighborhood of Crawford had a significant coefficient even though its mean house price was rather low.  I would think that that means that is an upcoming neighborhood.
