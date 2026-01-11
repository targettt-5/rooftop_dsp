# Rooftop Solar Potential Mapping — Delhi NCR

### Data Science & Machine Learning Project

This project estimates the rooftop solar energy potential of the Delhi NCR region by integrating
satellite-derived solar irradiation data, urban building footprints, and machine learning forecasting.
The objective is to support sustainable energy planning and solar-powered EV adoption.

---

## 📊 Executive Summary

- **Data**: 8 years (2015–2023), 4.8M+ buildings, 5 NCR cities  
- **Model**: Optimized Random Forest  
- **Performance**: R² = 0.984, RMSE = 274 MW  
- **2030 Forecast**: ~11.5 GW rooftop solar capacity  
- **Impact**: ~8 million tons CO₂ avoided annually

![Summary](../visuals/summary.png)

---

## 🗂 Data Sources

- NASA POWER — Satellite-derived solar irradiation
- OpenStreetMap — Urban building footprints
- MNRE Guidelines — Technical and economic parameters

---

## ⚙️ Methodology

1. Data acquisition and cleaning  
2. Feature engineering (climatic, urban, temporal)  
3. Baseline modeling (Linear Regression)  
4. Non-linear modeling (Random Forest)  
5. Scenario-based forecasting (2024–2030)

---

## 🤖 Model Performance

### Model Comparison using RMSE
![Model RMSE](../visuals/model_rmse.png)

### Model Comparison using MAE
![Model MAE](../visuals/model_mae.png)

The Random Forest model reduced RMSE by over **80%** compared to the linear regression baseline,
demonstrating strong non-linear modeling capability.  
Evaluation metrics (RMSE and MAE) were computed on held-out validation data to assess generalization
beyond the training period. The optimized Random Forest model was selected for scenario-based forecasting
due to its robustness.

---

## 🌆 Projected Rooftop Solar Capacity by 2030

### Optimal Future Scenario
![2030 Capacity](../visuals/city_capacity_2030.png)

Under the optimal future scenario, Delhi contributes the largest share of rooftop solar capacity,
followed by Gurugram and Noida. The results reflect differences in urban density and available rooftop
area across NCR cities.

---

## 🔍 Key Insights

- Seasonal effects explain a significant portion of annual variability, with summer months contributing disproportionately to total generation.  
- Urban density and available rooftop area were stronger predictors of solar capacity than short-term air-quality variations.  
- Technology efficiency improvements produced larger capacity gains than pollution-reduction scenarios.

---

## ⚠️ Limitations

- Partial reliance on synthetic historical data for long-term forecasting  
- Assumptions on policy adoption rates and technology efficiency  
- Rooftop orientation and shading effects not explicitly modeled  

---

## 🚀 Future Work

- Integrate real rooftop installation and utility-scale data  
- Improve pollution-feature sensitivity and temporal resolution  
- Incorporate spatial autocorrelation and neighborhood-level effects  

---

## 📌 Repository

All notebooks, data processing scripts, and detailed analysis are available in the GitHub repository.
