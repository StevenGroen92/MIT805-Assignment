# MIT 805 – Big Data Assignment (Transport Domain)

This repository contains code, notebooks, and outputs for **Part 1 & Part 2** of the MIT 805 Big Data assignment.  
The focus domain is **Transport**, using the **NYC Taxi & Limousine Commission (TLC) Trip Records** (Yellow, Green, and For-Hire Vehicles).

---

## 📊 Dataset

**Source:**  
- NYC TLC Trip Record Data (2019 – July 2025)  
  - [NYC TLC Open Data Portal](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)  

**Files downloaded:**  
- Yellow Taxi Trip Records (`yellow_tripdata_YYYY-MM.parquet`)  
- Green Taxi Trip Records (`green_tripdata_YYYY-MM.parquet`)  
- For-Hire Vehicle (FHV) Trip Records (`fhv_tripdata_YYYY-MM.parquet`)

**Size:**  
- Combined Parquet files (2019 – 2025/07): **~26 GB** on disk.  
- Rows: Billions across all three services.  

⚠️ **Note on GitHub Storage:**  
The full dataset (~26 GB) is **not uploaded** to this repository due to GitHub’s file size limits (100 MB per file, ~1 GB recommended repo size).  
Instead, the repository includes:  
- **Small sample files** in `data_samples/` for quick testing (<10 MB).  
- **Scripts and notebooks** to load and process the data.  
- **Links to official sources** (see above) so the full dataset can be re-downloaded if needed.  
- **Aggregated outputs and visualisations** generated for the assignment.  

---

## 📂 Repository Structure
mit805_transport/
├── README.md <- Project overview (this file)
├── requirements.txt <- Python dependencies
├── notebooks/
│ └── part1_explore.ipynb <- Data exploration (Part 1)
├── spark_jobs/
│ └── monthly_aggregates.py <- Spark/MapReduce jobs (Part 2)
├── data_samples/
│ └── yellow_sample_1k.parquet <- Tiny demo dataset
├── outputs/
│ ├── trips_per_month.csv <- Aggregated KPIs
│ └── charts/
│ └── trips_trend.png <- Visualisations
