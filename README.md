# MLInternshipTasks
This repository contains the Machine Learning Tasks I worked on while I was a Machine Learning Intern at Cognifyz Technologies.

# Step-by-Step Guide for Downloading the Shapefile for Task 4

## 1. Go to the Natural Earth Website
- Visit: [Natural Earth Downloads](https://www.naturalearthdata.com/downloads/)

## 2. Select the File Type
- Choose **"Cultural"** from the options, as the "low-resolution countries" shapefile falls under this category.

## 3. Download the Shapefile
- Look for the **"Admin 0 – Countries"** dataset.
- Click on the **"Download Countries"** button for the **1:110m** scale (this is the low-resolution version).
- This will download a zip file containing several files, including `.shp`, `.shx`, `.dbf`, and other necessary files.

## 4. Extract the Zip File
- Unzip the downloaded file to a folder on your local machine. It will contain files like `ne_110m_admin_0_countries.shp` and associated files.

## 5. Load the Shapefile into GeoPandas
- Specify the path to the extracted `.shp` file in your Python code:

```python
import geopandas as gpd

# Replace with the path to your downloaded shapefile
world = gpd.read_file('/path/to/ne_110m_admin_0_countries.shp')

# Now you can use the world GeoDataFrame for plotting
```

## Note
- Replace `'/path/to/ne_110m_admin_0_countries.shp'` with the actual file path on your system.
- Make sure all the associated files from the zip are in the same directory when you load the `.shp` file, as they work together.

This should allow you to proceed with loading the base map for your geographic analysis!

