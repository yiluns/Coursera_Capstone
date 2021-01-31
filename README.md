## IBM_Data Science_Capstone_Project:

## Segmenting and Clustering Toronto Neighborhoods.

### Project Goal:

For this project, I will explore, segment, and cluster neighborhoods in Toronto based on the most common category of the venues around each neighborhood. It is an explorative project incoporated with a bunch of techniques: _web-table-scraping, data clean-up and manipulation using Pandas, making API calls to Foursquare to retrieve location data,map visualization using Folium, K-Means clustering_.

### Data

The data required for this project is a table including all neighborhoods from Wikipedia. The link is here: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M. Because it is only a table, I will use Pandas library to scrape it and clean it up for requesting location for each neighborhood which is its latitude and longitude. Geopy package can find coordinates for each neighborhood. To better visualize each neighborhood, I will use Folium to build a map of Toronto and mark each neighborhood on this map.

### Methodology:

To explore each neighborhood and extract the venue information, I will make API calls to **Foursquare** to retrieve data such as venue name and venue category around each neighborhood. I will convert the json file into dataframe, extract the 10 most common types of venues for each neighborhood and use **_K-Means_** clustering to cluster neighborhoods based on their common types of venues. **_K-means_** is a simple but powerful model that is vastly used for clustering in many data science applications and is especially useful to quickly discover insights from unlabeled data. After performing K-Means clustering, I will examine each cluster to compare each cluster.

### Results:

I chose 4 clusters because from my visual inspection 4 clusters seem to make most sense. The dataset only has 90 neighborhoods after cleanup; due to some reasons such as limited location data or some other reasons, more than 85% of neighborhoods are clustered into one group.

From a quick review of these four clusters, I think the K-Means model performed pretty well in clustering neighborhoods. As we can see from Cluster 1, park is the most common category of venue for more than half neighborhoods. For the 5th through 7th most common category of venue, Fish Market and Filipino restaurants appear quite frequently. For Cluster 4, train station is the most common type of venue for both neighborhoods. However, like I mentioned, depending on locations, it might be hard to cluster neighborhoods in a single city because data is still limited, and neighborhoods in one city might be pretty similar. When I am reaching out to a bigger area or increasing the radius and limit when making API calls, I will definitely have some more clearly defined clusters.

### Conclusion:

This exploratory project grouped Toronto's neighborhoods into 4 clusters and provided some basic insights into each cluster's popular venues. Interestingly, most neighborhoods in Downtown Toronto tend to have similar types of venues such as cafe and pizza place. Even though this is a basic exploratory project, it taught me a lot of new techniques such as making API calls to external resources, converting json files into dataframes, visualizing maps using Folium. I will definitely try to explore more cities and locations using these techniques and generate some interesting findings!




