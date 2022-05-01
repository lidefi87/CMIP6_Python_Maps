# Accessing CMIP6 data with Python

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lidefi87/CMIP6_Python_SEE/HEAD)

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

Given that the above packages have a number of dependencies that may be complicated to install, I am also sharing a file called `environment.yml`, which has all the libraries you need to run this notebook in your own computer. You can install these libraries using the following line of code: `conda create -n my_new_environment -f environment.yml`. After installing this environment, you need to activate it with the following line: `conda activate my_new_environment`.

You can find additional information about environments in Python and how to create your own `yml` file [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file).

You can see this notebook in Binder by clicking [here](https://nbviewer.org/github/lidefi87/CMIP6_Python_SEE/tree/main/).
