# Accessing CMIP6 data with Python

This notebook shows you a basic workflow from accessing CMIP6 model data freely available from the Pangeo Cloud to creating simple maps and time series plots.

This Jupyter notebook uses the following libraries:
- xarray  
- numpy  
- intake  
- xmip  
- matplotlib
- cmocean
- cartopy
- os

Given that the above packages have a number of dependencies that may be complicated to install, I am also sharing two files which contain all libraries needed to run this notebook. If you are using a Windows-based machine use the `environment.yml`. If you are using Linux or macOS, use the `env_cross.yml` file, which is cross-platform compatible. We will use the `yml` file to create an [**environment**](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html#) which in simple terms is a folder containing Python packages that you need for a project.

To create these environments, I used [`Conda`](https://docs.conda.io/en/latest/), which is a popular software to manage packages and environments in Python. This means that you will neeed to install [`anaconda`](https://www.anaconda.com/products/distribution) or its minimal version, [`miniconda`](https://docs.conda.io/en/latest/miniconda.html) before you can recreate this environment in your system. You can check this [guide](https://docs.conda.io/projects/conda/en/stable/user-guide/install/download.html#anaconda-or-miniconda) to help you decide whether `anaconda` or `miniconda` is right for you. 

After `anaconda` or `miniconda` is installed in your computer, you can use the `yml` file to create an environment. Open the Anaconda Prompt, and type the following line: `conda env create -f ENVIRONMENT_FILE_HERE.yml`. Make sure to replace `ENVIRONMENT_FILE_HERE.yml` for `environment.yml` if using Windows or `env_cross.yml` if using other operating system. This line of code will create a new environment in your machine named `CMIP6_data`, which is the name I have given to this environment. If you prefer to use a different name, you can simply add a `name` argument to the line above, so it will look like this: `conda env create -n YOUR_ENV_NAME_HERE -f ENVIRONMENT_FILE_HERE.yml`. This will take a few minutes, so go grab a cup of coffee or tea in the meantime. Once the installation is completed, you can check that your environment has been successfully installed by running the following line: `conda env list`, which should give you a list of all environments you have available in your computer, which should include the environment you have just created. The last step is to activate the environment, which you can do by typing: `conda activate YOUR_ENV_NAME_HERE`.

You can find additional information about environments in Python and how to create your own `yml` file [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file).

*Note:*
The `cmip6_preprocessing` library was renamed `xmip` in 2022. This notebook and all supporting files have been updated to reflect this change.
