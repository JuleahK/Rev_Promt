# Data Analyst Technical Prompt


## Overview

This assignment involves forecasting sales data using historical data from one year of an e-commerece business. To complete the assignment, I was able to clean the data set in Python, dropping unnecessary columns (SKUS, descriptions, states, quantities, and unit prices), recategorized CustomerID to a category instead of an integer, filtered for positive sales only, and reindexed the dataframe to the date. After exporting the new csv, I was then able to model the data in Tableau. Using Tableau’s Analytics tab, I was able to create the images below. 

Tools:
- Python, for cleaning
- Excel, for visuals and initial forecasting
- Tableau, visuals and forecasting

Tableau’s forecasting tool allows for an Automatic Model (with or without seasonality) and uses exponential smoothing for trending and seasonal data, or a Custom Model in which trends and seasonality characteristics can be specified. 

Images 1 and 2 show the forecasts of number of sales by channel. The top sales producing channels are store (red), organic social media (yellow), and search engines (teal). The channels yielding the least results are display (blue) and mailing (green).

Image 1: Automatic Model https://public.tableau.com/app/profile/juleah/viz/Forecasting1_16281106356320/Dashboard2

![image](https://user-images.githubusercontent.com/78892035/128264578-f56be929-1564-472c-b65f-e34fcd61392b.png)

Image with trend lines only https://public.tableau.com/app/profile/juleah/viz/Forecasting4/ChannelsForecastTrendLines?publish=yes

Using this model, the forecast for stores and SEO trends up throughout Q1, while all others trend on a flat prediction. As most retailers can expect to see an element of seasonality in sales, this forecast may be a bit optimistic. It is evident in the historical data that sales volume has increased over the previous December of 2010 with the number of sales nearly doubling on some days in December 2011, however, the drop in sales between Q4 2010 and Q1 2011 is also evident and can almost be expected through seasonality. As sales gradually increase throughout 2011 and peak in December, we should expect to see the same lull for the following Q1, and then another gradual increase throughout 2012, again peaking in December. While there is not enough historical data here to accurately make this assumption, there is evidence of increased sales volume over last year’s December for this business, and while an infinite increase is unlikely, the business should expect to see more orders in 2012 if the trend continues. 

Image 2: Custom Model with no assessment for trends or seasonality

![image](https://user-images.githubusercontent.com/78892035/128381384-658fe2fa-12ac-47ca-9115-0b6a99edf728.png)

I changed the trend to none, and the seasonality to none, yielding a perhaps more realistic forecast. The trend line for each channel lies flat, with a prediction cone of 95%. The upper prediction level is lower than that of Image 1. 



Image 3: https://public.tableau.com/app/profile/juleah/viz/Forecasting2_16281106573330/Dashboard1

![image](https://user-images.githubusercontent.com/78892035/128264533-b85c1b79-2063-40f0-bc64-d2e812c78efb.png)

Image 3 shows the total sales trend for 2011, and the forecasted sales for Q1 2012. 

Image 4: https://public.tableau.com/app/profile/juleah/viz/Forecasting3/Dashboard3

![image](https://user-images.githubusercontent.com/78892035/128264448-f44fbae1-4021-476b-a838-edfc7e2a62bc.png)

Image 4 shows a side by side of sales per channel.

## Recommendations

In order to maximize sales in Q1 2012, the business should focus heavily on the top producing channels of store, organic social media, and search engine, respectively. By promoting the business through ads on top search engines, the business will gain more exposure to potential new customers. On the store level, the most basic form of preparation is to ensure that the store(s) is staffed and supplied adequately for the projected sales to come. Controlling the four walls of the store provides the strongest foundation for maximizing customers that come in, be it for the first time for repeat times. The store should properly train staff and monitor inventory to always keep coveted items available. For the organic social media channel, the business should ensure that posts are being made regularly, perhaps daily or weekly. Posts should be engaging and the business should, in turn, be engaging with their audience by responding to comments.

## Conclusion

Working on this assignment has been a great challenge. Forecasting and time series was not covered in my course so this has been my first experience with it. While I was able to find methods to us with Python and R, I’ve not yet been able to get the prophet package installed to R, and the Python notebook keeps crashing, presumably overloaded. 

After submition of this assignment, I welcome any feedback and advice for future forecasting tasks, and look forward to working with R and Python to complete them. 
