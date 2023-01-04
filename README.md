# Urban-Microclimates-and-Heat-Stress-Across-the-Continental-US
Fiker Zewdie's code for research project on the Urban Heat Island and Heat Indices.

This code was done for a project in 2020 aimed to look at four different US cities: Orlando, Atlanta, Houston, Phoenix. The csv files from the publicly available GridMET dataset contained temperatures from 1979-2019. One csv contained daily maximum temperatures and the other relative humidity temperatures. These cities were selected for their different climate seasons, with special consideration for heat index temperatures.

Heat index temperatures, also known as the feel-like or apparent temperature, is a calculated temperature used to understand what the dry bulb temperatures feel like accounting for the relative humidity. 

My code utilizes a dictionary that calculates the heat index given the maximum temperature and relative humidity. For each city the heat index temperature and maximum temperature are plotted against each other.

Some metrics calculated were the first heat day of the year, the last heat day of the year and the difference between the two is used to calculate the length of the heat exposure season. A linear relationship was drawn using scipy to calculate the change in the length of the heat exposure season.

Cooling degree days (cdd) is a metric for understanding projected energy consumption (in this case due to heat)

The threshold for cdd is 65°F or 18.33°C. The days that fell below this threshold were set to 0 to perform calculations on days that fell above this threshold only and a linear regression line was drawn to draw the increase in number of degrees above this threshold for each day (difference between threshold and temperature for the day).
