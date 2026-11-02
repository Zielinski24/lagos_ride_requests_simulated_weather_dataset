
# Simulated Weather Dataset

## Project Overview

This repository contains a simulated weather dataset prepared
for educational and data analysis purposes.

**Important:** This dataset is simulated and does not represent
a complete record of actual observed weather conditions.

## Dataset Information

- File: simulated_weather_data.csv
- Format: CSV
- Contents: Only the required dataset fields.
- Purpose: Data analysis and project exercises.

## Assumptions (Section 0.2)

1. [AREA_PRECISION = 3 ]          # decimals kept in lat/lng to define a "unique area" (3 decimals is about 110 m)
2. [REPEAT_MINUTES = 8]           # requests by the same user under 8 minutes after their first request are ignored
3. [FRAUD_METRES = 50 ]           # pickup and drop closer than 50 m are treated as fraud and ignored
4. [REPEAT_RULE_SCOPE = "user"]   # "user" = per user_ID (regardless of the area of origin); "global" = any user (removes most data; not recommended)

## Data Sources and Acknowledgements

Weather data credit: Open-Meteo.

Website: https://open-meteo.com/

## Disclaimer

This is a simulated dataset created for educational
and analytical purposes. It should not be interpreted
as verified real-world observations.
