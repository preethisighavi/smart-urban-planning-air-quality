# Smart Urban Planning: Optimizing City Layouts Based on Air Quality Trends

This project uses machine learning to analyze **air quality trends** and their relationships with urban factors such as **traffic**, **weather**, and **terrain**. The aim is to identify pollution hotspots and build predictive models that can support data-driven, sustainable city planning.

## Objectives
1. **Air Pollution Hotspot Identification**
   - Apply clustering techniques to detect regions with consistently high pollution levels and explore contributing factors.
2. **Predictive Modeling for Air Quality**
   - Train ML models to predict AQI (or AQI categories) using historical + urban/meteorological variables.
3. **Urban Planning Insights**
   - Interpret results to inform potential interventions (e.g., green space placement, traffic policy, zoning).

## Repository Structure
```text
smart-urban-planning-air-quality/
├── 00_data_prep.ipynb
├── 01_terrain_clustering_city.ipynb
├── 02_aqi_classification.ipynb
├── requirements.txt
├── README.md
├── .gitignore
└── data/
    ├── air_quality_final.csv
    ├── weather_final.csv
    ├── traffic.csv
    ├── terrain.csv
    └── merged_air_weather_traffic.csv
```

## Notebooks (Run in Order)
1. **00_data_prep.ipynb**
   - Cleaning / preprocessing
   - Merging datasets and preparing features
2. **01_terrain_clustering_city.ipynb**
   - Clustering analysis for hotspot identification
3. **02_aqi_classification.ipynb**
   - AQI modeling (classification) + evaluation

## Data
All datasets are in `data/`:

- `air_quality_final.csv` – Air quality indicators / AQI-related data  
- `weather_final.csv` – Meteorological features  
- `traffic.csv` – Traffic-related variables  
- `terrain.csv` – Terrain/land-use variables  
- `merged_air_weather_traffic.csv` – Merged dataset used for modeling  

## Setup
```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
# .venv\Scripts\activate  # Windows

pip install -r requirements.txt
jupyter notebook
```

## Notes
- The repo was cleaned for Git: removed macOS artifacts (`__MACOSX`, `.DS_Store`, `._*`) and replaced the Word `.gitignore.docx` with a proper text `.gitignore`.
