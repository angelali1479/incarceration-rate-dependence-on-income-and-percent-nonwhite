# Comparing Cupertino and Baltimore's Incarceration Rate Depending on Income and Percent Non-White Population

## Background

In my last project, I looked at Cupertino and Baltimore's incarceration rate in relation to income level and found correlations in the data. In my conclusion, I considered that there may be other variables at play that could be impacting the incarceration rate so I decided to bring in percent non-white as an additional variable to see if this factor will impact the incarceration rate. I am using similar data to see whether income and percent non-white population can predict the incarceration rate in both cities. It could be entirely possible that percent non-white is significant for one city and not for the other.

## Business Question

Can the incarceration rate in Cupertino and Baltimore be predicted by both household income and percent non-white population?

## Data

 - All datasets used were from [Opportunity Atlas](https://www.opportunityatlas.org/) and are in the repository above with the calculated datasets used as well.
  - [Baltimore Dataset](https://github.com/angelali1479/incarceration-rate-dependence-on-income-and-percent-nonwhite/blob/main/baltimore%20data%20final.xlsx)
  - [Cupertino Dataset](https://github.com/angelali1479/incarceration-rate-dependence-on-income-and-percent-nonwhite/blob/main/cupertino%20data%20final.xlsx)

## Data Analysis

In order to determine whether the two independent variables chosen are actually able to predict incarceration rate, we need to look at a multiple linear regression analysis of both city's datasets.

### Baltimore

![alt text](https://github.com/angelali1479/incarceration-rate-dependence-on-income-and-percent-nonwhite/blob/main/baltimore%20mult%20lin%20reg.png)

Here we have all the data from the multiple linear regression data analysis. As we can see, the R squared value is about 0.6 which means that about 60% of our data points can be predicted by the two independent variables. We also have a very small significance F, which means that the probability that our dependent variable won't be able to be predicted by the two independent variables is very small. The p-values for both independent variables are >0.05, meaning that both variables are significant enough to predict the dependent variable and we can use both independent variables in our final model. Using the coefficients from this data table, we can see that our formula would be: incarceration rate = -7.765E-07(Income) + 0.0278(Percent Non-White)

![alt text](https://github.com/angelali1479/incarceration-rate-dependence-on-income-and-percent-nonwhite/blob/main/inc%20rate%20inc%20-%20balt.png)

I used a scatterplot to visualize the way income predicts incarceration rate in Baltimore. As we can see in the graph here, there is definitely a clear shape and trend to the data points and the trendline on the graph is mostly in line with the data points. If we were to just look at the shape and not the linear trend line, we can surmise that the incarceration rate almost rises exponentially as income decreases. The p-value for this indepedent variable was very small, 76411E-025, so we can conclude that income is a significant predictor of incarceration rate.

![alt text](https://github.com/angelali1479/incarceration-rate-dependence-on-income-and-percent-nonwhite/blob/main/inc%20rate%20perc%20nonwh%20-%20balt.png)

I used a scatterplot to visualize the way percent non-white population predicts incarceration rate in Baltimore. As we can see in the graph above, the data points mostly follow a linear trend in line with the trendline on the graph. Compared to the scatterpltot of income, we can see that there is some more variance in the shape and data points; there are a few obvious outliers as well. The p-value for this independent variable was also very small, 4.9238E-17, which means that percent non-white population is a significant predictor of incarceration rate. However, judging by the difference in p-values (although very small) and the visual generated from the different data points, we can conclude that perhaps percent non-white population is slightly less strong of a predictor of incarceration rate.

### Cupertino


