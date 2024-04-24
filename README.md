## AidCompass, Your Disaster Relief Partner

This project uses machine learning and satellite imagery to better target disaster relief efforts. I focused on Typhoon Haiyan, which hit the Philippines in November of 2013. It broke records for having the highest wind speeds upon landfall and destroyed over 1 million homes.

After natural disasters, it's important to understand which areas suffered the most damage in order to prioritize relief efforts. Often times damage assessment maps are created by volunteers with the Humanitarian Open Street Map team who compare satellite imagery before and after the disaster and manually label each building with their evaluation of damage. However these maps are time and labor intensive to create, and not always accurate.

Studies have found that Open Street Map data often over-estimates damage in areas that are talked about in the news and under-estimates damage elsewhere.

## Goal

My goal was to create a model that could more quickly and more accurately identify the hardest hit areas in order to better target disaster relief.


## Applications

This sort of change detection model has many applications. For example, it could be used to identify illegal deforestation, monitor rising sea levels caused by global warming, or identify crop loss due to droughts or floods.

In the case of disaster relief as I've written about today, this model enables targeting of limited resources to ensure that structural building assessments, food, water, and other aid are going to the people who need it most.

-----
**Languages**: Python, JavaScript  
**Libraries**: Keras + TensorFlow, numpy, pandas, sklearn, rasterio, geopandas, shapely, opencv, matplotlib, seaborn  
**Methods**: Deep learning, classification (supervised learning)  

Replication notes:

- `google-earth-engine-satellite.js` pulls the satellite imagery from Google Earth Engine and should be run first.
- Building data shapefiles (grading maps) can be downloaded manually from the <a href="http://emergency.copernicus.eu/mapping/list-of-components/EMSR058">Copernicus Emergency Management Service website</a>.
- `0.0-data-prep.ipynb` is a precursor to two modeling notebooks. The latter two can be run independently of one another.
