# README: Preliminaries

Contact: <br/>
Jonathon Wright (jswright@tsinghua.edu.cn)<br/>
[jonathonwright.github.io](https://jonathonwright.github.io/)

Links to data files: 
- [oni.ascii.txt](https://cloud.tsinghua.edu.cn/f/4310a98472304798981e/) | 25K
- [tna.csv](https://cloud.tsinghua.edu.cn/f/1ea5017868cd4ae79625/) | 20K
- [tna_timeseries.nc](https://cloud.tsinghua.edu.cn/f/9cbbf1d3dafc417c9754/) | 158K
- [cams_compositionreanalysis_2003-2024.1m.nc](https://cloud.tsinghua.edu.cn/f/ba094a35311c47a381be/) | 287.9M
- [precip_CMAP_mon_1979-2024.nc](https://cloud.tsinghua.edu.cn/f/5f9c9efb912d45abb3ff/) | 16.6M
- [precip_GPCPv2-7_mon_1979-2024.nc](https://cloud.tsinghua.edu.cn/f/0278f6e49774480baa8f/) | 23M
- [sst_cobe2.atlantic.1x1.1850-2024.1m.nc](https://cloud.tsinghua.edu.cn/f/6c37b990ecee449b95b0/) | 67.4Μ
- [ERA5_surface_common-grid_monthly_pr_1940-2024.nc](https://cloud.tsinghua.edu.cn/f/6303990609024bfe9d4c/) | 41.8M
- [ERA5_surface_common-grid_monthly_t2m_1940-2024.nc](https://cloud.tsinghua.edu.cn/f/4310a98472304798981e/) | 43M
- [JRA-3Q_surface_common-grid_monthly_precip_1950-2024.nc](https://cloud.tsinghua.edu.cn/f/b2413778e75743c89927/) | 37M

The goal of these tutorials is to get you started with python and its applications in climate data analysis. If you are already using conda, you may want to use a clean environment to avoid conflicts. If you are not, instructions for getting started with [miniforge](https://conda-forge.org/download/) are provided in the links below.

Packages you will need:
- [xarray](https://xarray.pydata.org): our main analysis framework (note: installing xarray will also install [numpy](https://numpy.org/doc/stable/index.html), [pandas](https://pandas.pydata.org/pandas-docs/stable/index.html), and other useful packages)
- [netcdf4](https://github.com/Unidata/netcdf4-python) or [h5netcdf](h5netcdf): for reading data files
- [matplotlib](https://matplotlib.org/stable/index.html): required for plotting
- [cartopy](http://scitools.org.uk/cartopy/): required for plotting spatial distributions on maps
- [scipy](https://scipy.org/): for a broad suite of analysis tools

Optional packages for making nicer plots (I outline some uses of these in these examples):
- [seaborn](https://seaborn.pydata.org/)
- [colormaps](https://pratiman-91.github.io/colormaps/)
- [nc-time-axis](https://nc-time-axis.readthedocs.io/en/latest/): useful for plotting time series with date-aware axes

Optional packages for additional analysis
- [xeofs](https://xeofs.readthedocs.io/en/latest/)

All of these packages are easy to install with conda through [conda-forge](https://conda-forge.org/). Installers for miniforge (the current recommendation if you are just getting started with conda-forge) are located at https://conda-forge.org/download/, along with a link to [installation instructions](https://github.com/conda-forge/miniforge/blob/main/README.md). 

If you have already installed another form of conda (or mamba), you can access packages provided through conda-forge by adding the conda-forge channel at the command line:

```
$ conda config --add channels conda-forge
$ conda config --set channel_priority strict
```

or in your Anaconda Distribution software: 

1. Open Anaconda Navigator
2. Go to the Environments tab
3. Click the Channels button
4. Click the Add button
5. Enter the channel url: https://conda.anaconda.org/conda-forge/
6. Press Enter and then click the Update channels button
