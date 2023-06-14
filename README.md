# Final-Project-Tableau

## Intro
In movies and tv shows, there is always that one character that over exaggerates their fear and the risk of flying. Doing this project has taught me that it might not have been an over exaggeration after all.

The data I choose to work with is the Federal Aviation Administration's Wildlife strike dataset.  It contains records of wildlife strikes on planes from 2000 - 2015. The dataset contains information like the location, date and time, the effect it had, like cost and days it took to return the plane to working state, and species of the wildlife.

Why is this important?  Animals die every day (humans also eat them)

People might be more interested if human lives were lost regularly because of these strikes, but overlook the fact that even in the most simplistic cases animal lives are lost in a very disturbing fashion. To be clear, their lives are also important. If you look at the visual for forecasted strikes, you’ll notice that the number of strikes is only poised to increase. There has never been a better time to research and create measures to decrease wildlife strikes. And if that doesn't motivate you, maybe the fact that airlines get into a hurdle of legal issues and cough up some serious bills to fix the damage might.


## Dashboards 
 The first dashboard I created was to find patterns based on location so either by airport or state. You can filter with the map component and it will apply the filter throughout the dashboard. It computes a number of indicators. Feel free to look at the Tableau worksheet for a better understanding and is pretty much self explanatory. 


 The other dashboard I created was to find patterns based on month. You can filter the month through the regression plot and it will apply to the rest of the dashboard. One thing that stands out to me is that the 3rd quarter of each year has substantially more strikes than the rest of the quarters. 

## Results
(I went with option 2 with the FAA_data_subset)

 The main question that I sought to answer was if we can predict the cost incurred by the
species of the wildlife. Unfortunately, because species is a categorical variable, Tableau is unable to regress on it and find the correlation. I took it a step further and regressed it using python, and found that it explains less than 1% of costs. Why might that be? I can infer that it is because there is a more important factor like body mass of the animal or the part of the plane it came in contact with.

So what questions can the dashboards answer? Well we can find out which airports & states have the least strikes, and least costs. We can also compare the forecast of strikes for each airport, this can determine which airports are safer or at least in a safer location. 

If you look at the bar chart for the number of strikes based on phase of flight, you'll notice that most of the strikes happen when the plane is moving on the runway, and not parked. So reasonable to say the liability and fault lies on the airplane.  

One might also think we should change the time of our flights to the time where there are less strikes, which brings me to my next point. 

## Challenges 
The dataset only holds records of wildlife strikes, not a comprehensive record of all flights. This means that although we observe less strikes in a certain hour, it's possible that it could be at a higher % rate, if the time just has less number of overall flights. 

The dataset also does not contain information like the weight of the wildlife, direction the plane was heading, the destination, with part of the plane the wildlife came in contact with, and size of plane. If it did we could determine if those factors could explain the variability in Costs. 


## Future Goals
If I had more time and resources I would make the dashboard more easy to consume. Try to reconcile the subset with the parent data in hopes of being able to predict the cost of damage. 