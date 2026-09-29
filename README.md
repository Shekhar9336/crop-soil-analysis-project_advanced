# 🌾 Satellite & Soil Based Crop Recommendation System

Agriculture data-processing project: given a location, the system analyzes
real satellite imagery (NDVI), soil data, and weather to recommend suitable
crops and flag nutrient/weather deficiencies.

## Pipeline
Location → Sentinel-2 Satellite (real NDVI via Google Earth Engine) → Soil Data → Weather API → ML Model (Random Forest) → Crop + Deficiency Report

## What's Implemented
- Random Forest classifier trained on 2200 samples, 22 crops (~95%+ accuracy)
- Distance-based crop matching (alternate approach)
- Soil deficiency/excess detection with basic fertilizer suggestions
- REAL satellite NDVI via Google Earth Engine (Sentinel-2), using a Service Account
- Weather API integration (OpenWeatherMap) with automatic fallback to simulated data
- Multi-location tested (Punjab, Maharashtra, Kerala, Rajasthan)

## Tech Stack
Python, Pandas, Scikit-learn, Jupyter, Google Earth Engine, OpenWeatherMap API

## Files
- `Untitled.ipynb` — main notebook with full pipeline
- `Crop_recommendation.csv` — training dataset (Kaggle, 2200 rows, 22 crops)
- `real_satellite_report.csv` — multi-location output using real satellite data
- `requirements.txt` — Python dependencies

## Status
Core pipeline complete with real satellite + ML + deficiency detection.
Planned next: India Soil Health Card integration, web dashboard.
