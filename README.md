# nyc-taxi-demand-prediction

Predicting NYC Yellow Taxi Trip Demand
This project analyzes New York City yellow taxi trip data from November 2023 to September 2024 to forecast trip demand. By leveraging exploratory data analysis, geospatial visualization, time-series clustering, and machine learning, this work identifies key temporal and spatial demand patterns and develops a robust predictive model to provide actionable insights for urban transportation planning.


📜 Key Findings & Features

Temporal Analysis: The analysis uncovered distinct daily, weekly, and seasonal cycles in taxi demand. Demand peaks on Thursdays and during evening rush hours (18:00-19:00), while it subsides on weekends and during the summer months of July and August.






Geospatial Clustering: Using Time Series K-Means with Dynamic Time Warping (DTW), NYC taxi zones were grouped into five distinct clusters based on their demand patterns:




Cluster 0: High-demand business districts (e.g., Midtown Manhattan).


Cluster 1: Mixed-use urban zones with moderate, consistent demand.


Cluster 2: Residential zones with lower overall demand.


Cluster 3: Airport and transit hubs with unique travel schedules.


Cluster 4: Special activity zones with variable, event-driven demand.


Predictive Modeling: A cluster-specific XGBoost regression model was developed to forecast taxi demand.




Model Performance: The XGBoost model demonstrated superior performance, reducing prediction errors by approximately 30% compared to a Seasonal Naive baseline model across all clusters.


💾 Data Sources

Primary Dataset: NYC Yellow Taxi trip records from November 2023 to September 2024, provided by the NYC Taxi and Limousine Commission (TLC).


Supporting Dataset: A GeoJSON file containing the geographical boundaries for NYC Taxi Zones, sourced from NYC Open Data.
