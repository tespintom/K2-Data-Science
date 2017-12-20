# Cincinnati Real Estate Investment EDA

This project was created by necessity of an investor friend of mine.  As we sat side by side on couch, I saw that it took him about 30 minutes to research one investment property at time.	His process was the following:
	
	1. Find out which properties were going for auction at the weekly sheriff's sale.
	2. Map where the property was located
	3. Compare min bid with appraised value with Zillow's Zestimate
	4. Find out what yearly property taxes are for each property
	5. Then put everything into a single spreadsheet 

The main issue is that this process is very time consuming, as mentioned before, about 30 minutes per property (so it seemed!). But also, the information in the spreadsheet may be out of date by the time of the 11:30 am weekly Thursday auction.  Out of hundreds of properties that were going for the auction block, only a certain few were suitable to his risk tolerance; and in many occasions the desirable properties were taken off the sale do different circumstances.  

# Motivation

On what it seemed out of desperation :), my friend asked is this tedious process could be automated, and the short answer was yes!  
In this ongoing project, we are using a few Python Libraries in order to meet his need.  We are using Beautiful Soup in conjunction with Zillow's API to obtain Zestimate, tax information as well as Latitude and Longitude for geolocation purpose.  

We also used Pandas as well as visualization tools in order to find relationship as well as outliers.  

# Ongoing Research

As we continue to improve his wants, the idea is to host this project in a webapp where csv file can be uploaded in order to produce the final report that can be export it into a cleaned spreadsheet.  

We will implement predictive modeling in order to obtain a better understanding were max bid should be implemented.  

We would like to web scrape [Hamilton County Sheriff's Office](http://apps.hcso.org/Property.aspx) but we are running through some hicups.  
One major issue that we are running up against is it is fairly difficult to web scrape this webssite as there are no direct unique url to each of its links.













