# Pyber_Analysis

## Overview of the analysis: 

We were provided a variety of data related to ridesharing. One of the CVS files has info by city (city, number of drivers and city type), the other one has transactional or ride data (city, date, fare and ride id). Using this data we were asked to conduct some analysis and draw some conclusions. This analysis included:
(1) calculate the average fare per ride and average fare per driver for each city type
(2) create a multiple-line graph that shows the total fares for each week by city type

In order to accomplish this we used Pandas including the groupby(), count() and sum() funtions for the part (1) and the pivot() and resample() functions for part (2). Finally we used our Matplotlib learnings to create the final chart. 

## Results: 

The results of the analysis (1) are below:

![image](https://user-images.githubusercontent.com/96096924/150398289-436aaeb8-d405-4077-8da1-861e6a5dd198.png)

The image above shows that total rides and drivers go up the more urban the city which makes sense but also that the relationship with average fare and average fare per driver is inverse being higher in the more suburban and rural environments. Without further information one of the theories is that the trips are longer and thus the fares per trip are larger but we do not have enough information to assess if that is the only reason. Another theory is that the rides in relationship to drivers also goes up in the more rural areas thus the fares might be more competitive in those markets.  

The results of the analysis (2) are below:

![image](https://user-images.githubusercontent.com/96096924/150399100-0d169d3b-8977-4bc7-8500-59ec8da130d4.png)

In this chart you can see the total fare by city type over time. From these data you can observe that urban totals are higher than suburban and rural at any point in time, which clearly is driven by more drivers and more rides in these markets. You can also see seasonality of the Total Fares which is pretty stable , we don't observe any major peaks or valleys and any major observable differences across city types. The largest peak seems to be around late Febraury across city types.

## Summary: '

Based on the results above below are a few suggestions on how to reduce the disparity on total fares,  average fares and average fares per driver by city type:

(1) Clearly Urban Markets have an important driver saturation as you can see a low average per ride but even more importantly a very low average fare per driver , so I would first recommend to eliminate any incentives to drivers in this markets with the objective of reducing the count and if that does not work find other ways to be more selective in accepting drivers. 

(2) On the opposite axis clearly total drivers in comparison to rides is low in rural markets, so one hypothesis is that we could be leaving money on the table and rides due to not having enough drivers. So we would recommend to test increasing capacity to see if it leads to a higher overall revenue without significantly impacting the averages per ride and driver.

(3) In line with one of the other theories , the length and duration of trips could be driving the shorter averages in urban locations so maybe trying to implement a fixed fee in addition to the per mile or time fee in urban cities could help elevate those numbers a bit. The idea is to test and see if riders are sensitive to this or not. 
