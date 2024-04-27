# Wild Fires Analysis(Greece, Italy, Israel, Tunisia)

![Wild Fires Analysis Map](https://github.com/chrispassas98/Wild_Fires_Analysis/blob/main/photo/wild_fires.jpg?raw=true)

## Project Overview
This project analyzes recent forest fire data from Greece, Italy, Israel and Tunisia, based on satellite hotspots information provided by NASA. The data encompasses detailed measurements from three separate satellites, offering insights into the characteristics and impact of these fires.

NOTE: The project is not finished.

## Data Source

MODIS C6.1: Moderate Resolution Imaging Spectroradiometer
SUOMI VIIRS C2: Visible Infrared Imaging Radiometer Suite on the Suomi NPP (National Polar-orbiting Partnership) satellite
J1 VIIRS C1: VIIRS on the Joint Polar Satellite System-1
## Attributes Overview
Each record in the dataset includes the following key attributes:

- Latitude & Longitude: Center of the nominal 375 m fire pixel.
- Bright_ti4: Brightness temperature of the fire pixel in channel I-4, measured in Kelvin.
- Bright_ti5: Brightness temperature of the fire pixel in channel I-5, measured in Kelvin.
- Scan & Track: Pixel size along the scan and track, reflecting the actual pixel size which is approximately 375 m at nadir.
- Acquisition Date & Time: Timestamp of the VIIRS satellite overpass in UTC.
- Confidence: Quality indicator of the hotspot/fire pixel detection, ranging from low to high.
- FRP (Fire Radiative Power): Measures the pixel-integrated fire radiative power in megawatts (MW), crucial for estimating the fire's energy output and its contribution to local and global carbon budgets.
## Satellite Data Specifics
- Versioning: Indicates the data processing source and type—either Near Real-Time (NRT) or Standard Processing.
- Type of Detection: Classifies the source of fire or hotspots, such as vegetation fires, active volcanoes, other static land sources, or offshore detections.
- Day/Night: Indicates whether the detection was made during the day or at night.

## Analytical Goals
The primary aim of this project is to:

- Analyze the spatiotemporal distribution of forest fires.
- Assess the impact and intensity of fires through FRP analysis.
- Correlate satellite data with environmental factors to understand fire behavior.

## Data Accuracy and Uncertainty
This dataset incorporates a robust detection algorithm designed to minimize false alarms and optimize detection of small fires. However, FRP measurements come with inherent uncertainties, especially noted in areas affected by the South Atlantic Magnetic Anomaly, leading to potential false positives in night-time data. These inaccuracies have been accounted for in the NRT data provided by FIRMS.

# Source
https://www.kaggle.com/datasets/brsdincer/2000-2021-tunisiaisraelgreeceitaly-nasa/data
http://cedadocs.ceda.ac.uk/770/1/SEVIRI_FRP_documentdesc.pdf
