# tutorial-odc-stac

This tutorial will demonstrate how to load satellite imagery using `odc-stac`. At the end of the tutorial, you will have a Cloud Optimised GeoTIFF for an area of interest.

This tutorial will cover how to:
- Set up query variables to find satellite imagery that matches
    - an area of interest
    - a date range
- Connect to a STAC catalog and find data matching the query variables
- Load the data using `odc-stac`
- Visualise and export the data

## Steps

1. Clone the repository
```
git clone https://github.com/opendatacube/tutorial-odc-stac
```

Use conda to install the necessary packages from the `environment.yml` file:
```
conda env create -f environment.yml
```

2. Activate the environment
```
conda activate tutorial-odcstac
```

3. Open the `tutorial.ipynb` notebook and work through the cells.

## Area of interest
By default, this repository contains an `aoi.geojson` file that covers part of Wilkinkarra (Lake Mackay) in Australia.
A different area of interest can be chosen by replacing the contents of `aoi.geojson` with a new geojson.
