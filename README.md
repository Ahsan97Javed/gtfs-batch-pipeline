# 🚆 GTFS Batch Processing Pipeline & Transit Analytics Dashboard

A scalable, cloud-native batch processing pipeline for analyzing public transit data using GTFS (General Transit Feed Specification).  
This project leverages Google Colab, Google Drive, and Google BigQuery, with an interactive analytics dashboard built in Looker Studio.

---

### **Dashboard Description**

This dashboard provides an interactive overview of key public transit metrics generated from GTFS batch data.

**Features:**
- **Top 10 Most Popular Stops:** Highlights the busiest transit stops by scheduled stop times.
- **Top 10 Busiest Routes:** Displays the most active routes for operational insight.
- **Distribution of Routes Per Agency:** Shows how route management is distributed across transit agencies.
- **Trips Per Day of Week:** Reveals weekly demand patterns to optimize scheduling.

---

## 🛠️ Pipeline Architecture

- **Ingestion Microservice:** Reads and validates raw GTFS CSV files from Google Drive.
- **Preprocessing Microservice:** Cleans and standardizes the data.
- **Aggregation Microservice:** Computes key metrics and statistics in batch.
- **Output Microservice:** Writes processed data to Google Drive and Google BigQuery.
- **Visualization Layer:** Looker Studio dashboard connects directly to BigQuery for real-time analytics.
- **Version Control:** All code and documentation managed via GitHub.

---

## 🚀 How to Reproduce

1. **Prepare your GTFS files** and upload them to Google Drive.
2. **Run each Colab notebook** in sequence:
    - `01_ingestion_microservice.ipynb`
    - `02_preprocessing_microservice.ipynb`
    - `03_aggregation_microservice.ipynb`
    - `04_output_microservice.ipynb`
3. **Export aggregate results** to Google BigQuery.
4. **Connect BigQuery tables to Looker Studio** and build interactive visualizations.
5. **Schedule batch runs** using Colab scheduler or Google Apps Script.

---

## 📦 Data Access

Full GTFS datasets used in this project are stored on Google Drive for ease of access and to ensure reproducibility.

- [Google Drive – Full GTFS Dataset]((https://drive.google.com/drive/folders/1qtsPU90AbaDWaNW8MVw-7HBkKQLY0vLv?usp=drive_link))

## 📂 Project Structure
.
├── notebooks/
│ ├── 01_ingestion_microservice.ipynb
│ ├── 02_preprocessing_microservice.ipynb
│ ├── 03_aggregation_microservice.ipynb
│ └── 04_output_microservice.ipynb
├── diagrams/
│   ├── GTFS_Transit_Dashboard.png
│   ├── GTFS_Transit_Dashboard.pdf
│   └── architecture_diagram.png
├── docs/
│ ├── conception phase
│ ├── 
│ └── 
├── README.md
└── LICENSE
