# surfs_up
UW Data Bootcamp - Module 9

For this part of the Challenge, write a report that describes the key differences in weather between June and December and two recommendations for further analysis.

The analysis should contain the following:

**Overview of the analysis:** 

​		Helping W. Avy with the weather analysis data so he can decide if opening a surf and ice cream shop is a good idea in the prime location of Oahu. The particular ask right now is the weather analysis for the month of June and December.

**Results:** 

​		Before we jump in the results and analysis, couple of things to consider and contrast. We are using the data from 2010 to 2017. We are considering all the weather stations that means data is repeated from anywhere to 3-6times, a same date can be repeated. Lastly as seen from the summary picture below, our count analysis is not the same(1700 rows for June as compare to 1517 for December)

![June_Summary](C:\Users\Fahad.Rehman\Desktop\UW DataBootcamp\surfs_up\June_Summary.PNG)                ![Dec_Summary](C:\Users\Fahad.Rehman\Desktop\UW DataBootcamp\surfs_up\Dec_Summary.PNG)

​		From the weather analysis perspective, there's hardly a four Fahrenheit difference between June and December for 25% and 50% quartiles and merely a three Fahrenheit difference for mean, 75% and max values. 

​		It would be safe to say that Surfing activities and Ice Cream can be year round activity in Oahu

**Summary:** 

​		The first query I would like to use is the introduction of the most active weather station which is (USC00519281). The additional filter we would add is filter(Measurement.station == 'USC00519281'). This will give us more accurate summary analysis

​		The other variable I would combine with the temperature is the precipitation. Having a mean temperature of 74f doesn't tell you the whole story unless you bring the precipitation data in too. For that we will add a column i.e. Measurements.prcp

