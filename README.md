## IBM_Data Science_Capstone:

## Segmenting and Clustering Toronto Neighborhoods.

For this project, I will explore, segment, and cluster neighborhoods in Toronto based on the most common category of the venues around each neighborhood. 

The data required for this project is a table including all neighborhoods from Wikipedia. Because it is only a table, I will use Pandas library to scrape it and clean it up for requesting location for each neighborhood which is it latitude and longitude. Geopy package can find coordinates for each neighborhood. To better visualize each neighborhood, I will use Folium to build a map of Toronto and mark each neighborhood on this map.

To explore each neighborhood and extract the venue informationl, I will make API calls to Foursquare to retrieve data like venue information around each venue. I will convert the json file into dataframe, extract the 10 most common types of venues for each neighborhood and use K-Means clustering to cluster neighborhoods based on their common types of venues. Finally, I will examine each cluster. Because location data is still limited and all the neighborhoods are in Toronto, it is hard to recognize the difference between each cluster. 

Techniques used: _web-table-scraping, data clean-up and manipulation using Pandas, making API calls to Foursquare to retrieve location data,map visualization using Folium, K-Means clustering_.
