##### Justin Valdez 

# The Battle of Neighborhoods 

# Applied Data Science Capstone by IBM/Coursera

### Table of contents
* [Introduction/Business Problem](#introduction)
* [Data](#data)
* [Methodology](#methodology)
* [Analysis](#analysis)
* [Results and Discussion](#results)
* [Conclusion](#conclusion)

## Introduction/Business Probelm: <a name="introduction"></a>


### 1. Background
<u>**New York City (NYC)**</u>, The City, is the most poulous city in the United States. NYC has an estimated poulation of 8,398,749 distrubuted over about 302.6 square miles in 2018.

NYC is located at the southern tip of the U.S. state of New york, the city is the center of the New York metropitan area. With the amount of people in the metropolitan statistical area, NYC is one of the world's most populous megacities. Therefore, NYC is best described as the cultural, financial, and media capital of the world. The city influences commerce, entertainment, research, technology, education, politices, tourism, art, fashion, and sports.

NYC is set on one of the world's largest natural harbors, so it is composed of five boroughs - Brooklyn, Queens, Manhattan, the Bronx, and Staten Island - in which each is a county of the State of New York

### Objective
The aim of this report is to study and analyze the neighborhoods of New York City, group them into similar clusters and analyze those clusters to gather meaningful information. The data for New York has been touched upon on previous projects, but will be further finished.

### Target Audience:
The information provided by this project would be valuable for people who are interested or considering in relocating to different parts of the world. 

## 2. Problem Description


Now let me explain the context of this Capstone project through a scenario that can better be understood. Say you're preparing to move out from your parent's or guardian's home. You love your family, loved ones, and friends, but it's now time for you to move on to greater things and experience new ways of life. 

So, say you receive a job offer from a great company in *Manhattan, New York*. The company is offering a great pay and benefits. You have to decide to where in Manhattan you will stay and start your new life.

### 2.1 Data Description <a name="data"></a>
Considering the objective stated above, we can list the data sources used for the analysis below.

* New York City Data
  - The following Catalog Data page was scraped to pull out the necessary information: https://data.cityofnewyork.us/api/views/swpk-hqdp/rows.csv?accessType=DOWNLOAD
https://geo.nyu.edu/catalog/nyu_2451_34572


* Coordinate Data for each Neighborhood
  - The following csv file was used to get the latitude and longitude for NYC's Neighborhoods https://data.cityofnewyork.us/api/geospatial/tqmj-j8zm?method=export&format=Original
  
## 3. Methodology <a name="methodology"></a>

This part of the project represents the main component of the analysis where any exploratory data that was done, such as any inferential statistical testing that was performed, if any, and what machine learnings were used and why.
* Proccessing
  - Download and Explore Dataset
  - Transform Data Into Pandas Dataframe
  - Use Geopy Library in Order to get The Latitude and Longitude Values of New York City
  - Create Map of New York With Neighborhoods Superimposed on Top
  - Segmenting and Clustering Only the Neighborhoods in Manhattan
  - Retrieving the Geopgrpahical Coordinates of Manhattan
  - Visualization of Manhattan and the Neighborhoods
  
* Utilizing Foursquare API to Explore the Neighborhoods
  - Explore the First Neighborhood in the Dataframe
  - Retrieve the Latitude and Longitude Values
  - Finding the Top 100 Venues That Are in Marble Hill Within a Radius of 500 Meters
  - Send the GET Request and Examine the Results
  - Borrowing the get_category_type Function From the Foursquare Lab
  - How many venues were returned by Foursquare?
  
* Exploring 
  - Create a New Dataframe 
  - Check Size of the Resulting Dataframe 
  - Check How Many Venues Were Returned for Each Neighborhood
  - Determine How Many Unique Categories From the Venues can be Curated
  - New Dataframe Size
  
* Analyze Each Neighborhood in Manhattan
  - Group Rows by Neighborhood and Take the Mean of the Frequency of Occurrence of Each Category
  - Confirm New Dataframe Size
  - Display Each Neighborhood With the Top 5 Most Common Venues
  - Put This Data Into a Pandas Dataframe
  
## Results <a name="results"></a>


The goal of this analysis was to find out about the neighborhoods and their popular venues for a person planning to relocate within the city of New York.

As we analyzed the 5 clusters, we can determine a suitable neighborhood for a relocation. In fact, Cluster 2 seems to have the most venues if a person is interested in these places.

## Discussion


As seen in the table above, if a person wishes to move to New York, this can be a good option for them. For instance, this cluster contains restauraunts, gyms, etc. This is just one example of how our data analysis can help people relocate from one part of the world to another. 

## Conclusion <a name="conclusion"></a>


The world we live contains data everywhere we go, where many real-life problems or scenarios can be used to find solutions to these problems. This project showed that data was used to cluster neighborhoods in New York based on the most common venues in those neighborhoods. Therefore, someone that is planning to relocate where there are shops, restaurants, and gyms can use this data as a guide.

## References


* New York City Data
  - The following Catalog Data page was scraped to pull out the necessary information: https://data.cityofnewyork.us/api/views/swpk-hqdp/rows.csv?accessType=DOWNLOAD https://geo.nyu.edu/catalog/nyu_2451_34572


* Coordinate Data for each Neighborhood
  - The following csv file was used to get the latitude and longitude for NYC's Neighborhoods: https://data.cityofnewyork.us/api/geospatial/tqmj-j8zm?method=export&format=Original


* Foursquare API
  - The following site was used to get latitude, longitude, and data for venues: https://foursquare.com
