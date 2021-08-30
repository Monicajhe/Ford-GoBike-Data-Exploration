# Ford GoBike Data Exploration 
## by Jingjun He


## Dataset

This data set includes information about 2,506,983 individual rides made in a 
bike-sharing system Ford GoBike covering the greater San Francisco Bay area. 
The monthly data is provided by Bay Wheels and can be downloaded from their 
website. For the analysis, I download 12 monthly data from January 2019 to 
December 2019 to make a full year coverage. The attributes included duration, 
user type, start/end time, as well as additional information such as bike id, 
rental access method, start/end station, etc. Thirty-nine abnormal data points 
were removed from the analysis.


## Summary of Findings
 
Bike ride duration in the dataset take on a very large range of values, from 60 
at the lowest to 912110 at the highest. By removing outliers and plotted on a 
logarithmic scale, the distribution of bike ride duration look more like normal 
distribution with peak at little less than 550 seconds. Most bike rides are short 
trips. Majority of the bike users are subscribers(80.6%). Customer is 19.4% for 
those who do not subscribe.

In the exploration, I found that user type affects bike usage in number of rides 
and trip duration. Both types share some in common and have some difference. 
Although subscribers make a lot more trips than customers, customers generally 
take longer bike trip than subscribers. Both subscribers and customers take longer
trips during weekend than weekdays. Many commuters use the service for occasional 
short trips or to get to public transportation stops. Subscribers take most of their
trips around 7-9am(peak at 8am) and 4-6pm(peak at 5pm), typical commute hours. They
are probably commuters to work/school. Subscribers took more trips during the weekdays
and less on weekend. The usage trend for customers is relatively constant during the
week but with higher usage on Friday and Saturday. Customers show similar pattern with
subscribers on a daily basis expect that customers take less monring trips. The bike 
usage of both user types are affected by season. But usage for customers peaks in 
December, whereas for subscribers it is the opposite. Customers are probably tourist 
and occasional riders, who take the most rides in December due during the holidays. 
Houly average duration for customers are higher between 10am-5pm reaching its peak at 
2pm. The monthly average duration for subscribers looks stable during the year. The 
average duration for customers peaks at March and bottom at December.


## Key Insights for Presentation

For the presentation, I start by introducing the numeric variable duration in seconds
followed by other categorical variables user type and start time(separate hour, day,
and month in different columns). I'll plot to see impacts of user type on duration and
usage(in number of rides) and focus on how different groups of users use the service.