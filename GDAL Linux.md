---
created: 2023-08-15T14:36:40-05:00
updated: 2023-08-15T15:20:49-05:00
---
wget https://repo.anaconda.com/miniconda/Miniconda3-py311_23.5.2-0-Linux-x86_64.sh
bash Miniconda3-py311_23.5.2-0-Linux-x86_64.sh
yes

conda create -c conda-forge -n gdal gdal rasterio geopandas rio-cogeo
conda activate gdal
gdalinfo  --version


mkdir /work/my_project
setwd('/work/my_project')
renv::init()
Sys.setenv(RENV_PATHS_CACHE = '/work/my_project/renv/cache')
renv::use_python(type = 'conda', name = 'gdal')
install.packages(c("ncdf4"))

install.packages(c("units"))


install.packages(c("terra"))
install.packages(c("terra"))
install.packages(c( "rosm"))
install.packages(c( "gimms"))
https://docs.cloud.sdu.dk/hands-on/conda-rstudio.html