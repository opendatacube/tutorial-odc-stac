[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/opendatacube/tutorial-odc-stac/main?urlpath=%2Fdoc%2Ftree%2Ftutorial.ipynb)
# tutorial-odc-stac

In this tutorial we will use Python libraries to find and load land cover data from the freely available [Impact Observatory Annual Land Use Land Cover](https://planetarycomputer.microsoft.com/dataset/io-lulc-annual-v02) product.
After loading the data, we will export it as a cloud-optimised GeoTiff.
This will allow you to further view or work with the data in GIS software and other tools.

During the tutorial, we will:

* Specify our search in terms of:

  * what (data provider and satellite)
  * where (area of interest)
  * when (date range)
* Use `pystac-client` to connect to a Spatio-Temporal Asset Catalog (STAC) 
  endpoint and search for data matching our what, where, and when
* Use `odc-stac` to load the matching data into memory
* Visualise and export the data

You can see the full solution in `tutorial_solution.ipynb`.

## Option 1: Running in Binder
Binder provides an executable environment for running Jupyter notebooks. 
To launch a binder instance for this tutorial, click the button below:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/opendatacube/tutorial-odc-stac/main?urlpath=%2Fdoc%2Ftree%2Ftutorial.ipynb)

## Option 2: Running on a local computer

We provide an environment.yaml and requirements.txt file that detail the small number of required libraries for this tutorial. 
Follow the steps below to set up the tutorial on your own computer.

### 1. Clone the repository
Open a terminal and navigate to the directory where you'd like to keep the repository.
Then run
```
git clone https://github.com/opendatacube/tutorial-odc-stac
```

### 2. Install required packages

Set up a python environment with Python 3.9 or greater. 
Then, install the necessary packages with pip or conda:

**pip**
```
pip install -r requirements.txt
```

**conda**
```
conda env create -f environment.yml
```

Then, activate your environment if you haven't previously done so.

### 3. Open the `tutorial.ipynb` notebook and work through the cells.

The tutorial notebook contains empty cells for you to write code. 
The code you will need is available from the Open Data Cube docs [tutorial page](https://opendatacube.readthedocs.io/en/latest/tutorials/odc-stac.html).

## Area of interest
By default, this repository contains an `aoi.geojson` file that covers the southern part of Isla Isabela, one of the islands in the Galapagos.
A different area of interest can be chosen by replacing the contents of `aoi.geojson` with a new geojson.
