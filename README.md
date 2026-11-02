# Lagos Bike Ride Requests Simulated Weather Dataset

## 1. Project Overview

This project contains a simulated dataset of bike-ride requests in Lagos, Nigeria, for the year 2025. It is designed for data analysis and exploration of ride-request patterns, locations, and weather-related factors.

**Important:** This dataset is simulated and does not represent actual bike ride-hailing transactions or verified operational measurements.

## 2. Data Source

- Ride-request data: Simulated using the project's Python configuration.
- Weather data: Open-Meteo. Weather information is credited to [Open-Meteo](https://open-meteo.com/).

## 3. Section 0.2 – Simplifying Assumptions

The project uses the following three simplifying assumptions:

1. **Area precision:** Latitude and longitude are rounded to 3 decimal places to define a unique area. This is approximately 110 metres.
2. **Repeat requests:** Requests made by the same user within 8 minutes after their first request are ignored.
3. **Fraud detection:** Pickup and drop-off locations less than 50 metres apart are treated as fraudulent and ignored.

### Additional Simulation Configuration

- Simulation year: 2025.
- Assumed average raw ride requests: 1.6 per district per hour (pilot scale).
- Lagos weather reference coordinates: Latitude 6.5244, Longitude 3.3792.
- Repeat-request rule scope: Per user ID, regardless of the area of origin.

### Other Assumptions

- Lagos district characteristics and scores are assumed project inputs, not measured observations.
- Nigerian public holiday dates are approximate; Eid dates depend on moon sighting and should be verified.

## 4. Dataset Fields

The raw dataset contains the following eight fields:

| Field | Description |
|---|---|
| user_ID | Simulated user identifier |
| request_latitude | Latitude of the ride request |
| request_longitude | Longitude of the ride request |
| request_time | Date and time of the ride request |
| pickup_lat | Pickup latitude |
| pickup_lng | Pickup longitude |
| drop_lat | Drop-off latitude |
| drop_lng | Drop-off longitude |

## 5. Dataset File

The dataset is provided as a compressed CSV file:

`lagos_ride_requests_simulated.csv.gz`

Extract the `.gz` file before opening or analysing the CSV.

## 6. Disclaimer

This dataset is intended for educational, analytical, and project demonstration purposes only. All bike ride-request records are simulated. District scores and characteristics are assumptions and should not be interpreted as verified real-world measurements.
