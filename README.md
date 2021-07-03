# Basic analysis of the DeepMIP model database

<!-- 
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sebsteinig/HadGEM3-ancils/HEAD)
 -->

Collection of interactive jupyter notebooks to perform standard analysis and data 
extraction for climate model output stored in the DeepMIP data base. Notebooks use 
python 3.7. 

## Running the notebooks
Notebooks can be accessed and run by the Binder link above for convenience. They can also
be used as a template to perform further analysis locally. Easiest way is to install 
[conda](https://conda.io/projects/conda/en/latest/index.html) and create an environment 
`env_name` with:

```
conda env create --name env_name --file=environment.yml
``` 

using the `environment.yml` file from this repository. The notebooks can then be run 
interactively by typing:

```
jupyter notebook
```

or directly from the command line with:

```
jupyter nbconvert --to notebook --inplace --execute notebook_name.ipynb
```

## "extractSiteData.ipynb"

## other files

### Geographies
- herold_etal_eocene_topo_1x1.nc

### Paleogeographic rotation files

- LatLon_PD_55Ma_Herold2014.nc : 55Ma position in PD coordinates for Herold 2014 palaeogeography.
  (this means that you have a present day map showing at which lat-lon a point would be at 55Ma)
  
- LatLon_55Ma_PD_Herold2014.nc : PD position in 55Ma coordinates for Herold 2014 palaeogeography.
  (This is a 55Ma map showing from which lat-lon any point 'came' going back from present day)
