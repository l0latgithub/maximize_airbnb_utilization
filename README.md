### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

This notebook requires to install category-encoders (https://contrib.scikit-learn.org/category_encoders/) if you have not.

pip install category-encoders

Need to install a few packages to plot Boston Airbnb data on map and geoplot installation issue could refer to [here](https://github.com/googlecolab/colabtools/issues/85).

shapely needs to be reinstalled to use the same geos install as cartopy as [here](https://github.com/SciTools/cartopy/issues/871)

pip install geopandas

pip install mplleaflet

!apt-get install libproj-dev proj-bin proj-data

!apt-get install libgeos-dev

!pip uninstall -y shapely

!pip install --no-binary shapely shapely

!pip install cartopy

pip install geoplot

## Project Motivation<a name="motivation"></a>

As an Airbnb user, I am very curious about the utilization rate and profitability of Airbnb host. Thankfully, http://insideairbnb.com/ published some Airbnb data across the globe and it would help me to answer my own questions about Airbnb.

1.  What is key features to get high utilization?
 
 2. What can owner do to improve utilization?
 
 3. How to grow utilization for fresh Airbnb host?

## File Descriptions <a name="files"></a>

There are 2 notebooks available here to showcase work related to the above questions.

1. airbnb-github-v01.ipynb illustrates the large discrepancy of Airbnb host revenue even in similar location, athough property might have large differences. This leads to our focus: how to improve the occupancy rate for Airbnb host to increase revenue and profit 

2. boston_airbnb_plot.ipynb conducts data wrangling, feature engineerning, and model regression. Some interesting findings are obtained through this study and summarized in the post of results section.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://bmen689.medium.com/how-to-maximize-utilization-of-your-airbnb-e17850344854).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to http://insideairbnb.com/ for the data.  You can find the Licensing for the data and other descriptive information at the link available [here](http://insideairbnb.com/about.html#disclaimers).  Otherwise, feel free to use the code here as you would like! 

A customized LabelEncoder was used from https://www.kaggle.com/garethjns at [here](https://www.kaggle.com/garethjns/titanicsexism-fairness-in-ml).
