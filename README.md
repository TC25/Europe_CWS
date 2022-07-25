# Europe_CWS
Citizen weather station (CWS) data over Europe during the heatwave of July 2019. Specifics below:

Geojsons for the urban clusters, their buffers, and the decile regions for daytime and nighttime corresponding to MODIS Aqua and Terra land surface temperature (LST) observations are in the 'RegionsofInterest' folder.  

The 'DataSummaries' folder includes CWS measurements of air temperature (Temp) and relative humidity (RH) concurrent with MODIS LST observations for each day of July, 2019 (see date and Day fields). The satellite overpass time (MODIS_Time) and the sensor time (Sensor_Time) are included. Separate tables are used for each LST decile region, buffer, and corresponding to Aqua and Terra observations. 

The 'ClusterSummaries' folder includes the cluster-mean estimates of Temp and RH, as well as the corresponding Normalized Difference Vegetation Index (NDVI) from pixels overlaying the CWSs. Separate tables are used for each LST decile region and the buffer. Separate tables are used for each LST decile region, buffer, and corresponding to Aqua and Terra observations. 

The 'ClusterSummaries_percentile' folder includes cluster-scale estimates of the 95th and 98th percentile of CWS measured Temp, RH, and apparent temperature (HI). Separate tables are used for each LST decile region and buffer. 

The 'StationSummaries_percentile' folder includes estimates of the 95th and 98th percentile of CWS measured Temp, RH, and apparent temperature (HI), for each CWS considered here. Separate tables are used for the LST decile region and buffer. 
