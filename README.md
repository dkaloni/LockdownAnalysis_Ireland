# Impact of COVID19-induced Lockdown on Air Quality in Ireland

With the spirit of reproducible research, this repository contains codes required to produce the results in the manuscript:
    
> D. Kaloni, Y. H. Lee, S. Dev, Impact of COVID19-induced Lockdown on Air Quality in Ireland, *IEEE International Geoscience and Remote Sensing Symposium (IGARSS)*, 2021.
    
Please cite the above paper if you intent to use whole/part of the code. This code is only for academic and research purposes.

![gif11](/images/irelandNO2gif.gif)

*Time lapse of spatial distribution of nitrogen dioxide concentration for the case study of Dublin.*



![timeseries](/images/Dublin2020.png)
![](/images/Dublin2019.png)
*Impact of lockdown in the nitrogen dioxide concentration for the case study of Dublin*

 ## Code Organization
 All codes are written in `python3`.
 
 ### Dependencies
 The following libraries should be installed before the execution of the codes.
 + Xarray: `pip install xarray`
 + numpy: `pip install numpy`
 + pandas 1.0.5: `pip install pandas`
 + matplotlib: `pip install matplotlib`
 + netCDF4 1.5.3: `pip install netCDF4`
 + cartopy 0.18.0: `pip instal Cartopy`
 + termcolor 1.1.0: `pip install termcolor`
 + ipywidgets 7.5.1: `pip install ipywidgets`
 + glob2 0.7: `pip install glob2`
 + functools 0.5: `pip install functools`
 + scikit-image 0.17.2: `pip install scikit-image`
 + opencv-python 4.3.0.36: `pip install opencv-python`
 
### Data
The data source in this work is NASA's Goddard Earth Sciences Data and Information Services Center ([GES DISC](https://disc.gsfc.nasa.gov/)). We are releasing the processed data that we used in this work. You may download the processed data from [this Google Drive link](https://drive.google.com/drive/folders/1lC4DhQXn7p-c72P-AmAOU1bPa2UNBPYQ?usp=sharing). 

### Scripts

 + `CombiningNetCDFfiles_Dublin.ipynb`: Run this script to [combine netCDF files](http://nco.sourceforge.net/). This comes under preprocessing of data to obtain a publication quality dataset.  

+ `NO2_Ireland Plots.ipynb`: Run this script to obtain the distribution plots used in the paper. Contains time series line plot of daily average nitrogen dioxide concentration, bar plots of satellite data obtained from Sentinel-5P for average concentration of 15 days for year 2019 and 2020 and bar plot of fifteen days average concentration plots. It saves the plots as `.png` and `.pdf` format for future use in the same folder as the script.

+ `MapsfromNetCDFfiles.ipynb`: Run this script to retrieve, read, edit, store and plot netCDF files obtained from Sentinel-5P.


To explore Sentinel-5P in detail, follow Research and User Support of Copernicus at https://rus-training.eu/
