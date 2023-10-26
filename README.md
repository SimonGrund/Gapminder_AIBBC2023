# Gapminder World Data Analysis

## Introduction
Gapminder data set was made famous by Hans Rosling, who used to educate the public about World development (e.g. through TED talks). It contains various statistics for all countries in the World on demography, economy, and more. 

## Data
A small subset of the data is readily available in R through the Gapminder package. Load it using below code, or the load_data.R script in the code folder.

          install.packages("gapminder")  
          library(gapminder)
          d = gapminder 

The dataset in the gapminder R library contains 1,704 rows and 6 variables (country, continent, year, lifeExp, pop, and gdpPercap). Lots of additional data can be downloaded from the Gapminder website (see below) and potentially tied to the data from the Gapminder package. This requires a bit of data wrangling and handling of missing data in some cases.

## Potential questions:
Can you make interesting visualizations of the data that gives you a better understanding of differences in e.g. life expectancy and population size?
Can you predict life expectancy from the other variables, for a given year?
Do hierarchical modeling and adaptive priors perform better than modeling each country independently, with each their own pre-specified prior? If so, what works best:
Pre-specified identical priors for every country? 
An adaptive prior based on all countries in the World?
An adaptive prior based on all countries from within a continent?
Can you predict unseen (held out) data?
Can you estimate the population growth rate (potentially by transforming the population size) and its uncertainty?
Does hierarchical modeling help?

## Gapminder website:
A large number of additional statistics (for countries and years), such as CO2 emissions, can be downloaded from the Gapminder website:

  https://www.gapminder.org/data/
   
Scroll down to “Select an indicator” and choose what you are interested in. Then download as csv and import into R with, e.g., the read.csv2 command.
