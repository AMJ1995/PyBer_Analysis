# Analysis Overview

Myself and my colleague Omar have been given the task of creating a summary dataframe using data from a ridesharing company called Pyber. We focused on three different city types: Urban, Suburban and Rural. Using Pandas and Matplotlib along with our existing python knowledge, we were able to successfully analyze the rideshare data for these three city types and create a line chart to better help us understand this data.

# Analysis Results

We began by analyzing data given to us in a couple CSV files titled city_data and ride_data. Using pandas we were able to load these files onto our Jupyter Notebook. The first step was to find the total rides for each city type. We wrote a code to group the dataframe by "type" and our results were:
* 125 total rides in rural areas
* 625 total rides in suburban areas
* 1625 total rides in urban areas

This makes sense considering urban areas are highly populated and rural areas are typically low in population.
We then wrote a code to extract the total numbers of drivers for each city type. The code and it's output were this:

<img width="610" alt="Screen Shot 2022-04-09 at 11 38 30 AM" src="https://user-images.githubusercontent.com/100390727/162583165-1f80aaa1-7b80-48e6-bd82-dd56ffa10426.png">

As our output states:
* There are 78 total drivers in rural areas
* There are 490 total drivers in suburban areas
* There are 2405 total drivers in urban areas

Our next step was to find the total amount of fares (in $USD) for each city type. We wrote a similar code to extract this data and we found that:
* rural areas had total fares of $4,327.93
* suburban areas had total fares of $19,356.33
* urban areas had total fares of $39,854.38

We then used this data to find the average fare per ride for each city type. In our code we grouped by the city type and used the "mean()" function on the fare column of our dataframe. We found that:

* rural areas had an average fare of $34.63 per ride
* suburban areas had an average fare of $30.97 per ride
* urban areas had an average fare of $24.52 per ride

I'm assuming that rural areas had a higher fare average per ride due to rural areas being more spread out. Urban riders most likely had shorter rides since cities are more congested than bare rural areas.

We then found the average fare for each driver in all three city types. Our code and its output were:
<img width="735" alt="Screen Shot 2022-04-09 at 11 48 33 AM" src="https://user-images.githubusercontent.com/100390727/162583501-7c0c471b-ae35-4a00-b565-dac351dc2021.png">

Similar to the data we got for the average fare per ride above, rural drivers had the highest average fare and urban drivers had the lowest average fare.

We then created a new dataframe summary using this new data, and formatted everything so it looked cleaner and easier to read.
Then other dataframe was then created to look at the sum of the fares for each city type by the date and time of each ride. We then focused on two specific dates (1/1/2019 and 4/29/2019) and created a new dataframe for this info. The code and output for this looked like the following:
<img width="890" alt="Screen Shot 2022-04-09 at 11 59 23 AM" src="https://user-images.githubusercontent.com/100390727/162583874-893bd2cb-571a-4762-87bf-2480da4e4f87.png">

Ultimately, after these new dataframes were created we then put together a line chart to analyze our data and make it easier to understand. On our X axis was January through April of 2019, and our Y axis displayed the total Fare in $USD. Our chart looked like this:
<img width="1057" alt="Screen Shot 2022-04-09 at 12 02 03 PM" src="https://user-images.githubusercontent.com/100390727/162583981-5176fdfe-03c6-41ce-8ac8-9d636a0fa3b9.png">

# Summary
All in all, we were able to successfully analyze information about both riders and drivers of Pyber for urban, suburban and rural locations. Thankfully our use of pandas makes it much easier to get this information versus sifting through the large and confusing csv files. Matplotlib gives us the ability to plot this information into visually stunning charts so that this data can be conveyed more effectively.

There are 3 business recommendations that I would propose to the CEO of Pyber:
1) It would be helpful to see the distance and length of each ride for all city types. If we could analyze the average distance and the average duration of every ride we could then better analyze the data and potentially help the business grow with our findings.
2) Most modern rideshare services offer different options regarding the class of vehicle you can choose to ride in. For example, Uber has something called Uber Black which gives riders the choice of riding in a luxury car to their destination. If Pyber were to implement this option we could see in increase in total fares since these ride experiences are typically a few more dollars than rides in normal cars.
3) It would be interesting and beneficial to record the average ages of Pyber riders so that we could better understand the demographics of who is using this rideshare service. If we found this out then we could potentially market to our demographic and pull in more customers, increasing revenue.

