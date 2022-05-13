# Analysis of Weather Changes in the Past 80 Years in the State of Utah

## Intro

In this day and age, weather forecasts are important information to help us with several tasks such as what to wear or what preventive measures to take against an upcoming storm, to name a few. Just as essential is also improving our knowledge through weather analysis, which is the goal of this report. This report details on the weather changes in Utah over several in which three questions were addressed: 1. Is Utah drier than it was 80 years ago? 2. What is  the hottest year on record in Utah? 3. What is the coldest year on record in Utah? To answer these questions, meteorological elements such as temperature and precipitation data were collected from the archives of National Oceanic and  Atmospheric Administration (NOAA) and analysed to see how weather changed in Utah specifically in the past 80 years. The results depict important and helpful information about the weather changes that took place over the years, which maybe potentially useful to governmental organizations or private institutions working in this field of interest. 

## Methodology

The dataset collected are the Daily Summaries obtained through NOAA database the Global Historical Climate Network (GHCN). The Daily Summaries data is the daily land surface observations from around the world. According to the GHCN-Daily webpage, the GHCN-Daily data gets regularly updated and undergoes a variety of quality checks, making it suitable source of meteorological data for analysis. The Daily Summaries data sample collected from GHCN was obtained using the Climate Data Online search interface in the NOAA website. Using the search tool, all stations from Utah was chosen from the period between January 1940 to December 2020. The stations in Utah were sampled through cluster random sampling, followed by a convenience sampling from the randomly chosen cluster. Convenience sampling method was chosen in this case to meet the conditions that the station chosen had a wide data coverage range and that has been continuously recording data before 1950 in the Utah state for an accurate representation of Utah's weather over the years. The station that was picked was Alton, UT US station (Network ID: GHCND:USC00420086) with a data coverage of 99% that has been continuously recording meteorological data since 1915-05-01 until now. The dataset downloaded in csv file was analyzed in R programming software. The csv data file contained the daily precipitation data, maximum and minimum temperature data and temperature at the time of observation data. The precipitation data reflected mean precipitation value for each day for every year between 1940-2020, and the data ranged between 0-3.5. The maximum and minimum temperature values ranged from 3-99° F and -24-86° F, respectively. 

## Analysis

After the data was sorted, line-plot with trendline was used to demonstrate the precipitation (PRCP), max and min temperature data across all years between 1940-2020. Below is the plot using the precipitation data. It can be seen that the total PRCP values from each year differ significantly among each other, with highest value at 26.84 and lowest value at 5.33. Therefore, the wettest (26.84 total PRCP) Utah has been was in the year 2010 and the driest (5.33 total PRCP) in 1955. The second driest Utah was in the year 2020. But to the answer the question - Is Utah drier than it was 80 years ago? Following the trendline, it shows an increase in precipitation levels over the years. Bearing in mind that there are noticeable fluctuation in precipitation levels among the years, the trendline depicts that Utah has become wetter over the past 80 years. 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/105514187/168390187-3a4d3b4f-8e4d-4960-b5d8-c10def145a05.png">


Below is the plot of the mean maximum temperature in Utah from 1940-2020. The trendline shows an increase in the overall mean max temperature over the years. The lowest recorded mean max temperature can be seen at ~54.88° F, during the year 1993 and the highest recorded mean max temperature is seen at ~64.59° F on the year 2020, thereby indicating the hottest year on record in Utah. It is also important to mention that mean max temperature years 2017 and 2018 are very close to being the highest, however, mean max temperature on the year 2020 is the highest. 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/105514187/168390211-fb0e1df9-3408-40a0-aee5-1e64f127dd84.png">

Finally, to answer the question - What is the coldest year on record in Utah? Below is the plot that shows the annual mean min temperature plot for each year. The trendline shows an overall increase in mean min temperature over the years. However, the lowest mean min temperature was ~26.79° F on the year 1993, therefore, this suggest that 1993 is the coldest year on record in Utah. 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/105514187/168390238-ab307817-1e5f-4cf1-8e6a-a0344a030d1a.png">


## Conclusion

The analysis conducted using the dataset collected from Alton UT US station helped answer the three questions. However, there were many limitations that may indicate that the data is not entirely representative of Utah's weather changes over the past 80 years.The dataset collected had several "NA" or missing values, which may have given a skewed representation of the actual picture. This could be potentially solved by expanding the sample size to several station data to compare plots and confirm the true representation. Potential outlier values may also be noticed easily when comapared amonng many station data. Furthermore, the comparison of Utah's weather data with other nearby state's weather data, along with some literature knowledge on how typical weather tends to be historically in Utah and other nearby states, will potentially help identify a more accurate representation as well. Finally, this project could be improved through assessment of inter-analyst variability to check if there's a high degree of agreement between the results. 
