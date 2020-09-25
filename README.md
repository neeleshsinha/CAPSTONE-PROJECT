          CAPSTONE-PROJECT
[# IBM DATA SCIENCE PROFESSIONAL CERTIFICATE](https://www.coursera.org/professional-certificates/ibm-data-science)

# THE BATTLE OF NEIGHBORHOODS

By Neelesh Sinha

# INTRODUCTION
Our client came up with an idea of starting a food delivery service that he wants to start in the most
populated city suburbs of India for that our job is to find the best possible location for the service
because the future of his business depends on the initial profit of the business.

# PROBLEM
We have to find the most diverse and big cluster of restaurant neighborhoods for the location and
and for that we will go with k means clustering algorithm for optimal clusters.

# DATA

First, we will scrape the suburbs neighborhood data using beautiful soup from INTERNET and
use geopy for location coordinates also preprocess and clean the data, our four top cities are

# HYDERABAD
Source https://commons.wikimedia.org/wiki/Category:Suburbs_of_Hyderabad,_India

# BANGALORE
Source https://commons.wikimedia.org/wiki/Category:Suburbs_of_Bangalore

# MUMBAI
Source https://commons.wikimedia.org/wiki/Category:Suburbs_of_Mumbai

# CHENNAI
Source https://commons.wikimedia.org/wiki/Category:Suburbs_of_Chennai

# METHODOLOGY
1.Using Foursquare API to get different types of restaurant that exist within each city's
neighborhood. The Foursquare API allows application developers to interact with the
Foursquare platform. The API itself is a RESTful set of addresses to which you can send requests,
so there's really nothing to download onto your server. The Foursquare Places API provides
location-based experiences with diverse information about venues, users, photos, and check-ins.

2.Using folium to visualize the neighborhoods of cities to obtain an idea of the density. Folium is
a powerful Python library that helps you create several types of Leaflet maps. The fact that the
Folium results are interactive makes this library very useful for dashboard building.

3.Transforming data using one hot encoding dummy code based on food venue category and
grouping them and getting the frequency of each venue category in the neighborhood. After getting
the frequencies I identified cuisine clusters within each city and examine their frequency and
diversity.

4.I have used four k means cluster analysis for four cities to describe restaurant clusters within
these cities. Firstly, I used elbow method to determine the optimal number of clusters for cities to
indicate the number of clusters that lead to highest number of information gain for the dataset and
then used unsupervised k- means cluster analysis to find out how the neighborhoods were grouped
within each city based on food venue category as k means cluster analysis returns specified number
of clusters regardless of K’ optimality. After analysis cluster labels were obtained for each
neighborhood and content of each cluster was examined to create a dataset and top 15 frequent
venue categories for each cluster were plotted.

# DISCUSSION
FOR A FOOD DELIVERING COMPANY WE ARE TRYING TO FIND THE BEST
LOCATION IN THE MOST POPULATED CITY SUBURBS IN INDIA FOR THAT WE HAVE
TAKEN INTO CONSIDERATION BANGALORE,MUMBAI,HYDERABAD AND MUMBAI
AS OUR PRIMARY OPTIONS AND BASED ON DENSITY OF NEIGHBOURS AND
DIVERSITY IN CUISINE WE WILL PICK ONE OF THE CITY SUBURBS FOR OUR
BUSINESS. BASED ON THE NO. OF CLUSTER DECIDING OUR LOCATION WAS NOT
OPTIMAL SO WE EXAMINED THE CONTENT AND DIVERSITY OF CUISINES OF
CLUSTER TO CONCLUDE OUR RESULT.

# RESULT AND CONCLUSION
Based on the number of clusters we can see that Bangalore has the least number of clusters but the
no. of clusters is not the only good indicator of diversity in cuisine because a single cluster of
Bangalore has 75 categories of cuisine for that we have to examine the data of each cluster and
what they offer to customers. After my examination of cluster analysis, I have come to a conclusion
that Hyderabad is the most optimal location for starting food delivery service as it contains three
big unique clusters with much unique food venue categories and comparable neighbors to Chennai,
and Mumbai.
