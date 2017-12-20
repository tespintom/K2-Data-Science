# Bike Sharing Projection with Supervised Machine Learning

As part of the UCI ML Repository, bike sharing has become a hot commodity in metropolitan areas as well as college town.  Currently, there are about over 500 bike-sharing programs around the world composed of over 500 thousand bicycles. Today, there exists great interest in these systems due to their important role in traffic, environmental and health issues.

The idea behind this project is to understand need in order to know how many bikes are needed because if you have too few you’re not meeting demand and losing money. If a bike sharing company has too many bikes, you are not only paying for excess bicycles, but also for storage and maintenance.  For this project, you will predict the demand for bicycles in the near future.

# Dataset

This dataset has the number of riders for each hour of each day from January 1 2011 to December 31 2012. The number of riders is split between casual and registered riders, summed up in the count column.

	1. instant: record index
	2. dteday : date
	3. season : season (1:springer, 2:summer, 3:fall, 4:winter)
	4. yr : year (0: 2011, 1:2012)
	5. mnth : month ( 1 to 12)
	6. hr : hour (0 to 23)
	7. holiday : weather day is holiday or not (extracted from [Web Link])
	8. weekday : day of the week
	9. workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	10. weathersit :
		1: Clear, Few clouds, Partly cloudy, Partly cloudy
		2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	11. temp : Normalized temperature in Celsius. The values are derived via (t-t_min)/(t_max-t_min), t_min=-8, t_max=+39 (only in hourly scale)
	12. atemp: Normalized feeling temperature in Celsius. The values are derived via (t-t_min)/(t_max-t_min), t_min=-16, t_max=+50 (only in hourly scale)
	13. hum: Normalized humidity. The values are divided to 100 (max)
	14. windspeed: Normalized wind speed. The values are divided to 67 (max)
	15. casual: count of casual users
	16. registered: count of registered users
	17. cnt: count of total rental bikes including both casual and registered

# Approach 
The following questions were addressed in this project: 

	1. Feature engineering such as adding dummy variables to categorical variables when needed
	2. Scaling predictor variables for models such as knn
	3. Setting aside a testing and training set. Also, decide if you want to perform cross validation or set 	aside part of your training set as a dedicated validation set.
	4. Looking at and understanding feature correlation. You will likely not want to include registered or 	casual riders in your predictors feature because cnt = registered + casual.


