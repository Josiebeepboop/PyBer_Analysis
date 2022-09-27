# PyBer_Analysis

## Overview
PyBer is a ride-sharing app company. They have gathered their data and would like to analyze it to help improve access to their ride-sharing services and determine affordability for underserved neighborhoods.

---

## Purpose
To create a summary table of the ride-sharing data by city and plot a graph showing the total weekly fares for each city type. This will enable PyBer to make business decisions that will hopefully benefit their users going forward.

---

## Results & Analysis

The data provided can be found here: [Ride share data](Resources/ride_data.csv) and [City data](Resources/city_data.csv).

### Ride Share Summary

To create the summary table, the two datasets provided were merged together. Once merged, the required parameters were pulled and then used for calculation before entering the results into a new dataframe. From here, it is easy to see that urban cities have a higher volume of total rides (1,625) and drivers (2,405), which translates into higher total fares ($39,854.38) but lower average fares per ride ($24.53) and per driver ($16.57). There are thirty times less drivers in rural cities (78) and thirteen times less total rides (125) with a fares totalling $4,327.93. We see that the average fare per ride ($34.62) and per driver ($55.49) are the highest among the city types. Suburban city ride-share statistics sit in the middle of Rural and Urban cities with 625 total rides, 490 total drivers, and $19,356.33 total fares. Suburban cities have $30.97 average fare per ride and $39.50 per driver.

![Ride Share Summary Table](Analysis/ride-share-summary.png)

From this summary table we can also see that there are 1.6X more rides than drivers in rural areas. We also see a higher amount of rides versus total drivers in suburban areas (1.3X). In contrast, There are 0.7X less rides than drivers in urban areas.

### Weekly Fare per City Type

To visualize the weekly fares by city type, the merged dataset was used once again to group the rides by city type and date. The total fare was then calculated for each date and added to a new table. This table was pivoted to obtain a table with city types as the columns. A snapshot of the data from January 2019 to April 2019 was taken and resampled to provide weekly fares. This new table was plotted into the below line chart to visualize the weekly fares by city type from January to April.

![Weekly Fare per City Type](Analysis/PyBer_fare_summary.png)

In this line chart, we can see that the weekly fares for urban cities (close to $2,500 at times) are higher than for suburban (approximately $500 to $1,500) and rural cities (less than $500). If we combine this with the findings from the ride share summary table, it suggests that although there are more urban drivers, they are quite busy! The fares per week in rural cities sometimes tends towards the zero mark, which implies that there is very little activity at times.

---

## Summary Analysis

The data suggests that aren't many drivers signing up for ride-sharing in rural areas. It could be that the service is not well advertised in suburban and rural areas. Perhaps a more aggressive campaign in rural areas would attract more drivers to the service. The campaign could also be extended to the suburban areas to increase the driver count in these areas as well. By increasing the number of drivers, accessibility to the service can increase. 

There may be other reasons for the low demand. It can be argued that in suburban and rural areas, there is a higher population who already own cars. In this case, increasing attracting more drivers would not give the desired result. Although suburban and rural cities have lower total fares than urban cities they average more in fare per ride and per driver. This may mean that the service is too expensive when compared to using one's own car. To attract more users, perhaps lowering the fee in these areas would be a good option to increase ridership. 

Further, in rural and suburban areas, the length of the ride can be longer than in urban cities. Therefore, lowering the price based on the length of the ride may help to attract more customers. 

Finally, a survey should be used to determine if reasons for using or not using the service before and after the changes are implemented to properly monitor the improvements.