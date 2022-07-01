# PyBer Ride Share Analysis

## Project Overview
For this project the PyBer ride-share company requested a series of visualizations to help understand how ride numbers and costs relate to city size. Their goal is to help improve access to ride-sharing services and determine affordability for underserved neighborhoods. The company's 2019 ride data and city data were made available for analysis. 

## Resources
Data Sources: city_data.csv, ride_data.csv

Software: Jupyter Notebook 6.4.8, Python 3.10.5, Pandas 1.4.2, Numpy 1.21.5, Matplotlib 3.5.1, scipy 1.7.3

## Summary

### Ride Share Numbers
PyBer categorizes the cities they serve as urban, suburban, or rural based on population size. The table below provides an overview of city size as it relates to rides, drivers, and fare costs.

![image](https://user-images.githubusercontent.com/105830645/176822353-32947d51-2a11-4cf2-bf29-461df759d739.png)

It is important to note that while the effect of city size is immediately apparent in each category, a greater understanding of how these factors impact PyBer as a company can be gained using visual diagrams.

### 2019 Ride Share Visualizations
The following scatterplot shows how average fares relate to ride counts per city. Notice that average fare cost _generally_ decrease as the total number of rides in each city increases.
![Fig1](https://user-images.githubusercontent.com/105830645/176815387-918c0d7d-a671-46d8-8d02-059cdc9fae14.png)

#### Understanding Variance by City Size

The total number of rides in each city increases as city population size increases (as seen in the box and whiskers plot below), with the greatest variance in ride counts seen in the urban city category.
![Fig2](https://user-images.githubusercontent.com/105830645/176815499-0cc32869-6e83-4fa9-bcb1-42655b40161a.png)

When viewed as a whole, average fare costs by city type differ by a fairly small margin, but this gives an incomplete understanding of the data. The boxes below show how wide the range of average fares are for each city type. Rural cities have the largest variance in average fare costs, and this can be seen clearly using this type of diagram. Notice the least amount of fare variance is seen in suburban cities.
![Fig3](https://user-images.githubusercontent.com/105830645/176815740-53fe2b0c-ae3d-4e93-821a-2ea066df5820.png)

Driver counts also correlate to city size, with larger cities having more drivers to provide ride services. Notice in the box and whiskers plot below the largest variance in the number of drivers per city are in urban cities, while in rural cities there is very little variance, with an average of approximately 4 drivers per rural city.
![Fig4](https://user-images.githubusercontent.com/105830645/176816155-93cad828-58cd-4c14-84be-a64f027e6158.png)

#### Percentages by City Type

Looking at percentages by city type is another effective way of understanding the impact of city size on PyBer as a company. The pie chart below shows the effect of city size on total annual fares.

![Fig5](https://user-images.githubusercontent.com/105830645/176817064-80c48384-49ee-41e5-9a03-f22f2991f43f.png)

We see that rural cities make up less than 7% of total fares, while urban cities account for the majority of fares (62.7%). When comparing the total number of rides by city type the impact of city size becomes more significant, with urban cities accounting for the largest portion of rides (68.4%) and rural cities accounting for only 5.3% of the total rides (as seen in the pie chart below).
![Fig6](https://user-images.githubusercontent.com/105830645/176818042-fe8d4948-b00a-4992-9334-4e358e738a59.png)

The starkest contrast can be seen when comparing the percentage of total PyBer drivers by city type. Urban cities comprise the vast majority of PyBer drivers (80.9%), while rural cities comprise a bare fraction of PyBer's total drivers (only 2.6%!).
![Fig7](https://user-images.githubusercontent.com/105830645/176818818-7c209cf4-a704-4932-99d8-f56dab809ba1.png)

#### Weekly Fares Over a Defined Period
The previous visualizations gave an understanding of fare costs for all of 2019. To investigate how fares vary over time a subset of total weekly fares from January 1, 2019, to April 30, 2019, was created. The line graph below shows the fluctuations of fares over that period.

![Challenge](https://user-images.githubusercontent.com/105830645/176826945-a69161d7-2d01-419e-81e1-8538ce9f46f5.png)

- All city types experienced spikes in late February, coinciding with the US Valentine's Day holiday.
- Urban cities experience their lowest fares in early January, and their highest fares in late February and early March (with additional spikes in mid-March and early April).
- Suburban cities also experience their lowest fares in early January, with additional low points at the beginning of March and early April. A noticible increase in fares occured toward mid-to-late April. 
- Rural cities see their highest fares occur in late February and early March, with their lowest fare points in early January and early-to-mid February.

### Recommendations
PyBer is interested in expanding to underserved communities, and while these communities do not account for a large percentage of PyBer's overall business there are some data points of note. Fare cost did not have as much of an impact on rural city ride counts as it would immediately appear, as the top 3 performing cities had average fares of approximately $40, $26, and $35 respectively. Driver count did not impact the number of rides in rural cities either, as the top two performing cities had less than the average amount of drivers for this city type (<4). Rather than focus on driver recruitment or fare reduction in these areas, the next recommended step would be to investigate other factors in the top performing rural cities, such as geographic distribution of population, road conditions, and economic factors such as median income and number/concentration of businesses. 
