# Accessing CMIP6 data with Python

This notebook shows you a basic workflow from accessing CMIP6 model data freely available from the Pangeo Cloud to creating simple maps and time series plots.

This Jupyter notebook uses the following libraries:
- xarray  
- numpy  
- intake  
- cmip6_preprocessing  
- matplotlib
- cmocean
- cartopy
- os

Given that the above packages have a number of dependencies that may be complicated to install, I am also sharing a file called `environment.yml`, which has all the libraries you need to run this notebook in your own computer. To install these libraries you will need `anaconda` installed in your computer, which can download from [here](https://www.anaconda.com/products/distribution). Once you have `anaconda` in your computer, install the libraries in the `yml` file using the following line of code in the command line: `conda create -n my_new_environment -f environment.yml`. After installing this environment, you need to activate it by typing: `conda activate my_new_environment`.

You can find additional information about environments in Python and how to create your own `yml` file [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file).
