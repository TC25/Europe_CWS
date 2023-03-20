# Europe_CWS
Citizen weather station (CWS) data over Europe during the heatwave of July 2019. Specifics below:

Geojsons for the urban clusters (Cluster_vector.geojson; Clusters.geojson are their centroids), their buffers, and the decile regions for daytime (denoted by _d) and nighttime (denoted by _n) corresponding to MODIS Aqua and Terra land surface temperature (LST) observations are in the **'RegionsofInterest'** folder.  

The **'DataSummaries'** folder includes CWS measurements of air temperature (Temp) and relative humidity (RH) concurrent with MODIS LST observations for each day of July, 2019 (see date and Day fields). The satellite overpass time (MODIS_Time) and the sensor time (Sensor_Time) are included. Separate tables are used for each LST decile region, buffer, and corresponding to Aqua and Terra observations. 

The **'ClusterSummaries'** folder includes the cluster-mean estimates of Temp and RH, as well as the corresponding Normalized Difference Vegetation Index (NDVI) from pixels overlaying the CWSs. Separate tables are used for each LST decile region and the buffer. Separate tables are used for each LST decile region (p10 is 0 to 10th percentile or 1st decile, p20 is >10th to 20th percentile or 2nd decile, and so on), buffer, and corresponding to Aqua and Terra observations. 

The **'ClusterSummaries_percentile'** folder includes cluster-scale estimates of the 95th and 98th percentile of CWS measured Temp, RH, and apparent temperature (HI). Separate tables are used for each LST decile region and buffer. 

The **'StationSummaries_percentile'** folder includes estimates of the 95th and 98th percentile of CWS measured Temp, RH, and apparent temperature (HI), for each CWS considered here. Separate tables are used for the LST decile region and buffer. 

Explanation of critical column names:
- Cluster_ID: Unique ID of urban cluster
- ID, Sensor_ID: Both refer to unique ID of Nettamo sensor
- Perc: Percentile (or decile) region the data point belongs to
- View_time: Observation time in original time format
- date: Date of measurement
- LST: Land Surface Temperature
- Lat: Latitude
- Lon: Longitude
- Day: Day of the month
- MODIS_Time: Exact MODIS overpass time
- Sensor_Time: Sensor time closest to MODIS overpass time
- first: Can be one of the other columns depending on which variable was extracted using the map reduce operation; ignore this column
- Temp: Netatmo-measured air temperature
- RH: Netatmo-measured relative humidity
- indexMaster and moduleID: Internal indices added during processing; ignore for analysis

Contact tc.chakraborty@pnnl.gov for more details

# Relevant citations  

Venter, Z. S., Chakraborty, T., & Lee, X. (2021). Crowdsourced air temperatures contrast satellite measures of the urban heat island and its mechanisms. Science Advances, 7(22), eabb9569.  

Chakraborty, T., Venter, Z. S., Qian, Y., & Lee, X. (2022). Lower urban humidity moderates outdoor heat stress. AGU Advances, 3(5), e2022AV000729.
