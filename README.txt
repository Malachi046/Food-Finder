Food Finder


The data is from a non profit called falling fruit and can be downloaded from https://fallingfruit.org and has almost 2 million rows of locations with food all over the world. My goal is to help people access areas with plenty fresh food near them since traditional food manufacturing won't be operating as reliably. 



KNIME

To begin upload location.csv and types.csv to the KNIME project with location in the upper csv reader. 

The row filter retains all data points near the continental US(include southern Canada and northern Mexico) and the joiner adds the name of each food at a location. 

K-means then clusters the data into 400 clusters to allow a cluster to be relatively close to all areas, but k can be adjusted if you have better transportation.

The data is then saved in the CSV writer as ForagingData.csv with all the cluster assigned foods and ForagingClusters.csv with the centroid locations 


PYTHON

First download the files from the previous step and adjust their path in the code as necessary.

B1: 
Data is loaded and inputs for current latitude and longitude are made.
latitude range of data is [26-49] and longitude range is from [-67,-124]

B2:
Nearest cluster to location is identified

B3:
Directions to the nearest cluster are made

B4:
All the food in the nearest cluster is listed and nearest point in the cluster is found

B5:
Directions to the nearest food source is made




