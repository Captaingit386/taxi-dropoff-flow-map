# Taxi Drop-off Prediction & Flow Map Dashboard

This project analyzes taxi mobility using pickup signals and vehicle telemetry to model drop-off behavior and visualize pickup → dropoff flows on an interactive map. It includes a Python notebook for data processing/modeling and a Node.js dashboard for exploration.

## Key features

- Feature engineering from telemetry fields (GPS validity, location, timestamp, speed, heading, for-hire light, engine status)
- Baseline ML model (Random Forest) to infer drop-off outcomes
- Generates an Origin–Destination (OD) flow dataset (pickup zone → dropoff zone)
- Interactive map dashboard to explore flows by pickup area

## Tech stack

- Python: pandas, numpy, scikit-learn
- Backend: Node.js, Express
- Frontend: Leaflet, PapaParse

## Project structure

```text
.
├── ML.ipynb
├── README.md
├── LICENSE
└── nodejs/
    ├── server.js
    ├── package.json
    ├── public/
    └── data/
        └── pickup_dropoff_flows.csv

## Run locally

### 1) Start the dashboard

```bash
cd nodejs
npm install
npm start

// here is the web side for raw data
https://traffic.longdo.com/opendata/probe-data/
```
