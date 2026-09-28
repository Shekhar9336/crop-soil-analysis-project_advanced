# Satellite & Soil Based Crop Recommendation System

Agriculture data-processing project: given a location, the system analyzes
satellite (NDVI), soil, and weather data to recommend suitable crops and
flag nutrient/weather deficiencies.

## Pipeline
Location → Satellite (NDVI) → Soil Data → Weather API → ML Model (Random Forest) → Crop + Deficiency Report

## Tech Stack
Python, Pandas, Scikit-learn, Jupyter, OpenWeatherMap API, SoilGrids API

## Files
- `Untitled.ipynb` — main notebook with full pipeline
- `Crop_recommendation.csv` — training dataset (Kaggle, 2200 rows, 22 crops)
- `final_analysis_report.csv` — sample multi-location output

## Status
Core ML pipeline + deficiency detection complete. Real satellite imagery (Google Earth Engine) planned next.
