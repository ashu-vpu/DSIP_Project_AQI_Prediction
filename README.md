# DSIP_Project_AQI_Prediction
Topic :
Forecasting India's Air: AQI Patterns and Real-Time Pollution Alerts

**Team members :**
Tony P Joy (tonyjoy@iisc.ac.in)
Vivek H N (vivekhn@iisc.ac.in) 
Neeraj Shete (neerajshete@iisc.ac.in)
Ashutosh Mishra (ashutoshmish@iisc.ac.in)


**Problem Statement:**
Globally, air pollution is a silent killer. The air pollution levels in India are among the highest in
the world, posing a heavy threat to the country's health and economy. All of India’s 1.4 billion people are
exposed to unhealthy levels of harmful pollutants - emanating from multiple sources. In this project we are
trying to analyse and understand the levels of major air pollutants and the resultant AQI (Air Quality Index)
across the major cities in India. Through this analysis we intend to identify the patterns and observations related
to the AQI that can provide the data backing to prepare a search/ warn system for the citizens on the air quality
at a given date and time of the year and remind them about wearing their N95 masks.

**Problem motivation: **
While the depleting air quality is a growing concern in India it doesn’t seem to get the
required attention both from the responsible sector and the sufferer sector. We believe that the relevant data and
live warnings – when incorporated with the daily digital tools like news feeds, tweets and maps can help to
bring the desired emphasize and drive actions.

**Dataset :**
The dataset comprises air quality measurements and meteorological data collected from six major Indian cities: Bengaluru, Chennai, Delhi, Hyderabad, Kolkata, and Mumbai. It covers a significant period with hourly data points, resulting in a total of 262,944 entries. The columns include 26 variables, split into pollutant levels, weather-related metrics, and timestamps for each observation.

Here's an overview of the columns:

Key Attributes:

City and Timestamp: These provide location and time information for each reading, essential for temporal and spatial analysis.

Pollutant Levels: The dataset includes a variety of pollutants, some commonly monitored in air quality indices:

PM2.5 and PM10: Particulate matter at different sizes (µg/m³), which are significant indicators of air quality.
NO, NO2, and NOx: Nitrogen oxides (µg/m³ or ppb) that are byproducts of combustion and are harmful in high concentrations.
NH3, SO2, CO: Other gases such as ammonia (NH3), sulfur dioxide (SO2), and carbon monoxide (CO) in respective units, indicating levels of various airborne compounds.
Ozone: Ozone levels (µg/m³), another important metric in assessing air quality.
Benzene, Toluene, Xylene, O Xylene, Eth-Benzene, MP-Xylene: Volatile organic compounds (VOCs), measured in µg/m³, often resulting from industrial and vehicular emissions.
Weather-Related Variables:

AT (Air Temperature in °C): Provides temperature data.
RH (Relative Humidity %): Measures humidity.
WS (Wind Speed in m/s) and WD (Wind Direction in degrees): Give insights into wind conditions, which affect pollution dispersion.
RF and TOT-RF (Rainfall in mm): Includes both current and cumulative rainfall, which can influence pollutant levels.
SR (Solar Radiation in W/mt²): Indicates the solar energy received, impacting atmospheric reactions.
BP (Barometric Pressure in mmHg): Pressure data that can affect pollutant concentration.
VWS (Vertical Wind Speed in m/s): Represents the vertical movement of wind, useful for advanced analysis on pollutant movement.
Missing Data
There are some columns with considerable missing data, notably:

Xylene (µg/m³), O Xylene (µg/m³), Eth-Benzene (µg/m³), and MP-Xylene (µg/m³) have lower non-null counts, indicating possible data gaps for these VOCs.
VWS (m/s) and AT (°C) also have a significant portion of missing values, which might require special attention during analysis.
This dataset provides a comprehensive foundation for understanding urban air quality trends, correlations with weather conditions, and evaluating city-wise differences in pollution levels.

**Acknowledgements : **
https://airquality.cpcb.gov.in/ccr/#/caaqm-dashboard-all/caaqm-landing/caaqm-data-repository

**Notes** : 
**The notebook "Data_Science_IP_Project_checkpoint1_EDA.ipynb" contains interactive plots. To view all the EDA plots - please open the notebook in Colab or python runtime.**

** To Save a Model for future use **
# Save the model to the specified directory
joblib.dump(rf_rscv, "/content/drive/MyDrive/DE_Scale_Project/DSIP_rf_rscv_model") 
