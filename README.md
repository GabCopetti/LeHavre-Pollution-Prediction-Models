***
# Predicting PM10 concentration in Le Havre, France
***

**To read a version of the notebook, wihout needing to install RStudio, a .pdf is available.** 

Models were created in **R** to predict the concentration of particulate matter pollutants, with diameter smaller than 10 micrometers, in the city of Le Havre, France. The *rep* data set from the VSURF library was used.

According to data set description, PM10 concentrations were measured by Air Normand, from 2004 to 2006. The monitoring station is situated in an urban site, close to traffic, and considered the most polluted in the region. The concentrations of pollutant gases, as well as the associated weather data provided by Meteo France, were used as input variables.

The data set was split into Learning and Test sets before modelling. Variable selection was performed using random Forests with the VSURF package. Linear Regression, Decision Tree and Random Forest models were constructed and compared by calculating the Root Mean Squared Error (RSME) and the Mean Absolute Error (MAE). 

 

# Installation

RStudio 2023.09.1+494 was used, available for download and installation <a href="https://dailies.rstudio.com/version/2023.09.1+494/" target="_blank">here</a>. R version was 4.2.3.

To install required packages from .lock file, use the command **renv::restore()**.
