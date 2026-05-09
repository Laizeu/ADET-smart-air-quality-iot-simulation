# Smart Air Quality IoT Monitoring System  
### Multi-Station Urban Air Pollution Simulation for Metro Manila

MO-IT148 · Application Development and Emerging Technologies  
Mapúa Malayan Digital College · Term 3 SY 2025–26  

---

## Project Overview

This project simulates a **Smart City Air Quality Monitoring System** inspired by real-world environmental networks used in cities.

It models how distributed IoT sensors collect environmental data across different urban zones in Metro Manila, generating structured datasets for analysis of air pollution patterns across time and location.

The system focuses on **spatial (location-based)** and **temporal (time-based)** variations in air quality, comparing high-traffic corridors against low-emission green zones.

---

## Monitoring Stations

The simulation uses five representative urban monitoring locations:

| Station ID   | Location                 | Traffic Profile | Zone Type          |
|--------------|--------------------------|-----------------|-------------------|
| STN-EDSA-01  | EDSA-Guadalupe          | Very High       | Transport Corridor |
| STN-ESP-02   | España-UST              | High            | Academic Corridor  |
| STN-C5-03    | C5-Pasig                | Mixed           | Arterial Road      |
| STN-QUI-04   | Quiapo-Plaza Miranda    | Very High       | Urban Core         |
| STN-UPD-05   | UP Diliman              | Low             | Green Baseline     |

---

## System Architecture

The system follows a **three-layer IoT data model**:

1. **Monitoring Stations** – Physical urban locations  
2. **IoT Sensors** – Data collection devices per station  
3. **Sensor Readings** – Time-series environmental measurements
4. **Analytics Layer** - Processes raw data and computes Air Quality Index (AQI)  
5. **Output Layer** - Structured datasets exported as CSV and JSON for analysis  

This structure mirrors real smart city deployments where multiple sensors feed data into centralized analytics systems.

---

## Parameters Simulated (13 Fields per Reading)

### Air Quality Metrics
- PM2.5
- PM10
- CO (Carbon Monoxide)
- NO₂ (Nitrogen Dioxide)
- O₃ (Ozone)

### Environmental Conditions
- Temperature (°C)
- Humidity (%)
- Wind Speed (m/s)

### Derived Metrics
- Air Quality Index (AQI)
- AQI Category:
  - Good
  - Moderate
  - Unhealthy for Sensitive Groups
  - Unhealthy

### Metadata
- Sensor ID
- Station ID
- Location
- Timestamp

---

## Tech Stack

- Python
- Pandas
- NumPy
- Jupyter Notebook

---

## Key Features

✔ Multi-station IoT simulation  
✔ Traffic-based pollution modeling  
✔ Realistic environmental variability  
✔ Time-series dataset generation  
✔ AQI computation and classification  
✔ CSV and JSON export support  

---

## Output Files

The system generates structured datasets:

- `stations.csv` → Monitoring station metadata  
- `sensors.csv` → IoT sensor registry  
- `sensor_readings.csv` → Main time-series dataset  
- JSON equivalents for API-ready structure  

---

## Methodology

### Traffic-Based Pollution Modeling
Pollution levels are dynamically adjusted based on traffic intensity:
- Very High traffic → increased PM2.5, CO, NO₂
- Low traffic → baseline environmental conditions

### Environmental Influence
- Wind speed reduces pollutant concentration
- Humidity affects particulate suspension
- Temperature influences dispersion behavior

### AQI Computation
AQI is calculated in Python using weighted pollutant contributions to simulate real-world air quality indexing behavior.

---

## Real-World Relevance

This system reflects principles used in modern smart city environmental monitoring systems such as:

- Urban air quality tracking networks
- IoT-based pollution monitoring systems
- Environmental data analytics platforms

Inspired by smart city frameworks used in:
- Singapore environmental monitoring systems
- Seoul air quality tracking networks

---

## Learning Objectives

This project demonstrates:

- IoT system architecture design
- Environmental data simulation
- Time-series dataset generation
- Smart city modeling concepts
- Data-driven environmental analysis

---

## Limitations

- Simulated data only (no physical sensors)
- Simplified AQI calculation model
- No real-time streaming infrastructure
- No government API integration

---

## License

For academic use only  
MO-IT148 · Mapúa Malayan Digital College
