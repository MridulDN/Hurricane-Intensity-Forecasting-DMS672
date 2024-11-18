**Hurricane Intensity Forecasting**

This project integrates machine learning with socio-demographic analysis to forecast hurricane behavior and identify vulnerable regions. The project focuses on Hurricane Ian, which struck the U.S. in September 2022 and aims to improve disaster preparedness through accurate path and intensity predictions combined with targeted vulnerability assessments.
A project report has also been included, kindly refer to it for detailed explanation.

**Objectives**
Vulnerability Analysis:
Identify counties most affected by Hurricane Ian.
Use socio-demographic data (e.g., income, vehicle availability, age distribution) to compute aid scores for disaster management.

Hurricane Path and Intensity Forecasting:
Develop an LSTM-based model to predict hurricane path and intensity using sequential data.
Evaluate the model's performance with different sliding window sizes.

**Methodology**

Phase 1: Vulnerability Analysis
Data Sources:
Hurricane Cone and Track Data: Extracted from the National Hurricane Center (NHC).
Demographic Data: Census data (age, income levels, vehicle ownership).
Geographic Data: Census TIGER/Line shapefiles for spatial intersections.
Key Metrics:
Vehicle Availability Index: Prioritizes evacuation needs.
Income-Based Vulnerability Score: Quantifies economic resilience.
Aid Need Score: Combines age, sex, and population factors.

Phase 2: LSTM-Based Prediction
Model: Long Short-Term Memory (LSTM) network.
Data Preprocessing:
Feature engineering: Calculated derivatives for wind speed and storm movement.
Sliding window approach to capture temporal dependencies.
Evaluation:
Mean Absolute Error (MAE) for path and intensity predictions.
Compared performance with varying window sizes.

**Results**

Vulnerability Analysis:
Identified the top 5 counties needing aid using geographic and demographic data.
Visualized vulnerable regions using GIS tools like QGIS and Folium.
LSTM Model:
Achieved accurate path and intensity predictions for Hurricane Ian.
Enhanced predictions by incorporating temporal features such as storm trajectory rates.

**Challenges and Future Work**

Challenges:
Limited dataset: A small number of advisories constrained model performance.
Optimization of window size: Conflicting results for path and intensity predictions.
Future Improvements:
Incorporate additional hurricane data to improve generalization.
Use environmental data (e.g., sea surface temperature) with CNNs for multimodal learning.
Explore probabilistic forecasting methods for handling uncertainties.

