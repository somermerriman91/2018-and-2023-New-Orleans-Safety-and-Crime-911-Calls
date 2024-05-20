# 2018 New Orleans Safety and Crime Incident Data Analysis and Visualization 

### Project Overview
The primary objective of this project is to conduct a comprehensive analysis and visualization of incident data reported to the Orleans Parish Communication District (OPCD) for the year 2018. The insights generated from this analysis have the potential to significantly impact decision-making processes related to resource allocation for the New Orleans Police Department (NOPD) and other relevant stakeholders. The project aims to improve public safety, reduce crime rates, and enhance the overall effectiveness of law enforcement operations. Furthermore, it aspires to foster transparency and accountability in resource allocation practices.

### Project Goals

### Data Cleaning and Preprocessing:

Open Nola911Calls2018.ipynb in Jupyter Notebook and follow the markdown instructions. 
Break down coordinate values into usable Latitude and Longitude values to facilitate heatmap visualization.
Group reported incidents into appropriate incident/crime categories to uncover geographic and temporal patterns.
Identify and remove burglar alarm-related records, which are deemed unreliable for the project's objectives.
Your final dataframe should match nolacrimecleanest.csv.

### Exploratory Data Analysis (EDA): (to be completed)

Conduct a thorough exploration of the dataset to understand the nature and distribution of incidents reported to OPCD in 2018.
Examine the spatial and temporal aspects of incidents to identify hotspots, trends, and anomalies.

### Tableau Visualization

#### Connect to data sources.
Connect to 'nolacrimecleanest.csv' and 'NOPD_Police_Districts.shp'.
Join the two data sources within the logical layer on "District" = "District".

<img width="724" alt="image" src="https://github.com/somermerriman91/2018-New-Orleans-Safety-and-Crime-911-Calls/assets/143425643/0cb2e9fb-b215-4917-bace-9edc2e180bc1">

#### Create a static KPI with summary statistics on incident count by category in percentage form for the entire dataset. 

<img width="991" alt="image" src="https://github.com/somermerriman91/2018-New-Orleans-Safety-and-Crime-911-Calls/assets/143425643/38c3c135-fd5c-43f5-b6e8-36febc643e24">


#### Create a District filter as an interactiveness feature.

<img width="308" alt="image" src="https://github.com/somermerriman91/2018-New-Orleans-Safety-and-Crime-911-Calls/assets/143425643/a4c7f65d-1fab-4143-9547-94b45f124c24">


#### Create a bar chart for incident category that is affected by filter action. Make category bars highlightable to affect heatmap and line chart.

Utilize "Count" measure and "Incident Category" and "District" dimension.

<img width="779" alt="image" src="https://github.com/somermerriman91/2018-New-Orleans-Safety-and-Crime-911-Calls/assets/143425643/da9cf0e1-f6d7-4993-82a9-0ebf04c84b0e">


#### Geospatial vizualization: create a heatmap that is affected by both District filter and highlight feature of bar chart. 

Utilize "Count" measure and District dimension.

<img width="479" alt="image" src="https://github.com/somermerriman91/2018-New-Orleans-Safety-and-Crime-911-Calls/assets/143425643/11a909a1-20cc-4044-a38b-69cc74a619f5">


#### Temporal Visualization: create a line chart of the "Time" value of Date/Time vs. "Count" measure.  This should also be affected by both the District filter and hightlight feature of the bar chart. 

Analyze the temporal patterns of incidents to identify peak hours of the day with higher activity.

<img width="506" alt="image" src="https://github.com/somermerriman91/2018-New-Orleans-Safety-and-Crime-911-Calls/assets/143425643/56db0b52-d3b3-47b9-8c1d-993531d05e03">



The finished product should look visually appealing and engage users. [Tableau Public Link](https://public.tableau.com/app/profile/elizabeth.merriman/viz/2018NewOrleansSafetyandCrime911Calls/2018NewOrleansSafetyandCrime911Calls?publish=yes).


#### Resource Allocation Recommendations:

Based on the analysis results, provide actionable recommendations for resource allocation within NOPD and related organizations.
Suggest adjustments to police presence, patrol routes, and response times to improve public safety.



## Files list


| Data file | Source | Notes    |Provided |
|-----------|--------|----------|---------|
| `nolacrimecleanest.csv` | Local File | Cleaned Data | Yes |
| `nolacrimeraw.csv` | [Kaggle](https://www.kaggle.com/datasets/ericgoldberg/safety-and-crime-911-calls-new-orleans-2018) | Raw Dataset | Yes |
| `NOPD_Police_Districts.shp`| [ArcGis.com](https://hub.arcgis.com/maps/d9d7c99ddf4645b38d72b09f06dffa66/explore?location=30.021106%2C-89.882950%2C11.60) | Geospatial File for District visualization | Yes |




### Software Requirements

- Tableau 2023.3.0
- Python 3.11.4
  - `pandas` 1.3.5
- Jupyter Notebook 7.0.6






