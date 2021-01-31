## IBM_Data Science_Capstone_Project:

## Segmenting and Clustering Toronto Neighborhoods.

### Project Goal:
For this project, I will explore, segment, and cluster neighborhoods in Toronto based on the most common category of the venues around each neighborhood. It is an explorative project incoporated with a bunch of techniques: _web-table-scraping, data clean-up and manipulation using Pandas, making API calls to Foursquare to retrieve location data,map visualization using Folium, K-Means clustering_.

### Data
The data required for this project is a table including all neighborhoods from Wikipedia. The link is here: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M. Because it is only a table, I will use Pandas library to scrape it and clean it up for requesting location for each neighborhood which is its latitude and longitude. Geopy package can find coordinates for each neighborhood. To better visualize each neighborhood, I will use Folium to build a map of Toronto and mark each neighborhood on this map.

### Methodology:
To explore each neighborhood and extract the venue information, I will make API calls to Foursquare to retrieve data such as venue name and venue category around each neighborhood. I will convert the json file into dataframe, extract the 10 most common types of venues for each neighborhood and use K-Means clustering to cluster neighborhoods based on their common types of venues. K-means is a simple but powerful model that is vastly used for clustering in many data science applications and is especially useful if you need to quickly discover insights from unlabeled data.

Finally, I will examine each cluster. Because location data is still limited and all the neighborhoods are in Toronto, it is hard to recognize the difference between each cluster. 


