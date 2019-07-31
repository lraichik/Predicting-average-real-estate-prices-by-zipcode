# Overview  

In this project I am working with data from Zillow to try to predict sales prices in the future. The goal is to see which zipcodes would make the most sense to invest in with regards to profit and return on investment in 12 months.  

I will look at all three of these parameters when making my recommendations for these reasons: 
  
**Profit** - Tells us in dollar amount how much we estimate can be made as well as confidence intervels with a min and max profit margin.  
  
**Return on investment** - Percentage that can be gained, this metric can tell us if the amount we are able to make is a small or big precentage. This will help with understanding that even if a big profit can be made, this may be more of a risk with regards to small market swings. 

  
### City  

I will be looking at zipcodes in the city of Chicago, of which there are 41 zipcodes.   

<details><summary>Map of zipcodes in Chicago</summary>
<img src='Chicago_zipcodes.png'>
</details>

## Findings

Here is the graph for what I would consider is the best zipcode that I found:

<img src='Chicago_best.png'>

As can be seen, at the 12 month mark the growth is not by too much and the lowest price is below the original buying price.

Here are the 10 best zipcodes by profit:

<img src='Chicago_profit.png'>

Here are the 10 best by return on investment:

<img src='Chicago_roi.png'>

Here is what each column refers to:  
**known_RMSE**: RMSE for the data that I have, checked against the predictions made.  
**Forecast_2019_04**: A forecast for 12 months in the future  
**confid_min and confid_max**: The confidence min and max  
**profit**: The dollar amount of profit based on the predicted value in 12 months.  
**roi**: Return on investment percentage  
**2018_04_price**: The price at the buying time, which was the last date in the data.  
**max_loss**: The 2018 price minus the min in 12 months, if this is a positive number then there is a loss, if this is a negative number then there is no predicted loss, even if sold for the lowest predicted price in 12 months.  
**loi**: Loss on investment percentage, as above, if it is positive then there is a loss, if it is negative then there is no predicted loss, even if sold for the lowest predicted price in 12 months  

As can be seen the return on investment is low. Even in the best one, with a %9 return, the actual profit is low.  

Also, there is a chance of losing money on each one of these, with the max loss on investment percentage sometimes higher then our mean return on investment percentage.

For what it is worth, here is a picture showing what I would consider the top 4 zipcodes:

<img src='5_best.png'>

## Recommendations

Due to this, and the fact that there are other costs invlolved as well beyond just the buying a selling price, I cannot recommend investing in the Chicago real estate market for selling houses in 12 months.  


## Future Work

I would suggest looking into other areas to invest in.

See my notebook on Kings County, NY [here](Brooklyn.ipynb), and the Readme on it [here](Brooklyn.md).