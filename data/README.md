# Data

-   The dataset comprises weather forecast data gathered over 16 months from 167 cities across the United States. It's aimed at analyzing the accuracy of high and low-temperature forecasts and understanding the regional variances in forecast accuracy. The data has been sourced from the USA National Weather Service and processed by the team at the Saint Louis University Department of Mathematics and Statistics.

# Codebook for Weather Forecast Accuracy Dataset

## Variable Names and Descriptions:

### For `weather_forecasts.csv`:
-   **date**: The date the forecast and observation are described for.
-   **city**: Name of the city.
-   **state**: State or territory where the city is located.
-   **high_or_low**: Indicates whether the forecast is for the high or low temperature of the day.
-   **forecast_hours_before**: The number of hours before the observation (one of 12, 24, 36, or 48).
-   **observed_temp**: The actual observed temperature on that date (high or low).
-   **forecast_temp**: The predicted temperature on that date (high or low).
-   **observed_precip**: The observed precipitation on that date, in inches; some observations lack an indication of precipitation, while others explicitly report 0.
-   **forecast_outlook**: An abbreviation for the general outlook, such as precipitation type.
-   **possible_error**: Either (1) "none" if the row contains no potential errors or (2) the name of the variable that is the cause of the potential error.

### For `cities.csv`:
-   **city**: Name of the city.
-   **state**: State or territory where the city is located.
-   **lon**: Longitude of the city.
-   **lat**: Latitude of the city.
-   **koppen**: Köppen climate classification.
-   **elevation**: Elevation of the city in meters.
-   **distance_to_coast**: Distance to coast in miles.
-   **wind**: Mean wind speed.
-   **elevation_change_four**: Greatest elevation change in meters out of the four closest points to this city in a collection of elevations used by the team at Saint Louis University.
-   **elevation_change_eight**: Greatest elevation change in meters out of the eight closest points to this city in a collection of elevations used by the team at Saint Louis University.
-   **avg_annual_precip**: Average annual precipitation in inches.

### For `outlook_meanings.csv`:
-   **forecast_outlook**: An abbreviation for the general outlook, such as precipitation type.
-   **meaning**: The meaning of the forecast outlook abbreviation.

## Data Types:

### For `weather_forecasts.csv`:
-   **date**: date
-   **city**: factor
-   **state**: factor
-   **high_or_low**: factor
-   **forecast_hours_before**: integer
-   **observed_temp**: integer
-   **forecast_temp**: integer
-   **observed_precip**: double
-   **forecast_outlook**: factor
-   **possible_error**: factor

### For `cities.csv`:
-   **city**: character
-   **state**: character
-   **lon**: double
-   **lat**: double
-   **koppen**: character
-   **elevation**: double
-   **distance_to_coast**: double
-   **wind**: double
-   **elevation_change_four**: double
-   **elevation_change_eight**: double
-   **avg_annual_precip**: double

### For `outlook_meanings.csv`:
-   **forecast_outlook**: character
-   **meaning**: character


