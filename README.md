***
# Predicting PM10 concentration in Le Havre, France
***

**To read a report, wihout needing to install RStudio, the .pdf is available.** 

Models were created in **R** to predict the concentration of particulate matter pollutants, with diameter smaller than 10 micrometers, in the city of Le Havre, France. The *rep* data set from the VSURF library was used.

According to data set description, PM10 concentrations were measured by Air Normand, with the associated weather data provided by Meteo France, from 2004 to 2006. The monitoring station is situated in an urban site, close to traffic, and considered the most polluted in the region. The following variables are available:

- PM10: Daily mean concentration of $\text{PM10}$, in $\mu g/m^3$.

- NO, NO2, SO2: Daily mean concentration of $\text{NO}$, $\text{NO}_2$ , $\text{SO}_2$ in $\mu g/m^3$.

- T.min, T.max, T.moy: Daily minimum, maximum and mean temperature, in degree Celsius.

- DV.maxvv, DV.dom: Daily maximum speed and dominant wind direction in degree.

- VV.max, VV.moy: Daily maximum and mean wind speed, in m/s.

- PL.som: Daily rainfall in mm.

- HR.min, HR.max, HR.moy: Daily minimum, maximum and mean relative humidity, in %.

- PA.moy: Daily mean air pressure in hPa.

 - GTrouen, GTlehavre: Daily temperature gradient in degree Celsius in the cities of Rouen and Le Havre, respectively.

The data set was split into Learning and Test sets before modelling. Linear, Decision Tree and Random Forest models were constructed and compared by calculating the Root Mean Squared Error (RSME) and the Mean Absolute Error (MAE). Variable selection was performed using random Forests with the VSURF package.

 

# Installation

RStudio 2023.09.1+494 was used, available for download and installation <a href="https://dailies.rstudio.com/version/2023.09.1+494/" target="_blank">here</a>. R version was 4.2.3.

To install required packages from .lock file, use the command **renv::restore()**.
