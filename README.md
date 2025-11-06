# ⚡ Optimal Electric Vehicle Charging Station Placement in India 🚗🔋

### 📘 Project Overview
This project aims to identify **optimal locations for EV charging stations across India** using **Machine Learning** and **Geospatial Analysis**.  
It integrates **population**, **EV infrastructure**, and **geographic data** to predict EV station density and suggest new station placements based on underserved regions.

---

### 🧠 Objectives
- Analyze and visualize the current distribution of EV charging stations in India.  
- Predict EV density (`EVs_per_million`) using regression models.  
- Identify states and regions requiring new EV charging infrastructure.  
- Visualize optimal placement zones using geospatial mapping and buffer analysis.

---

### 🧩 Dataset
**Sources Used:**
- 🇮🇳 *Indian EV Charging Stations Dataset*
- 📊 *Population Data* – Census of India (2021 projections)  
- 🗺️ *Geospatial Data* – GADM v4.1 India shapefile  
- 🧮 Final dataset merged using Pandas and GeoPandas with features:
  - `State`, `Population`, `EV_Stations`, `EVs_per_million`, `Geometry`

---

### ⚙️ Technologies Used
| Category | Tools / Libraries |
|-----------|------------------|
| **Programming** | Python (3.12) |
| **ML Models** | Linear Regression, Random Forest, XGBoost |
| **Libraries** | Pandas, NumPy, scikit-learn, XGBoost |
| **Visualization** | Matplotlib, Seaborn, GeoPandas, Shapely, Folium |
| **Environment** | Google Colab |
| **Deployment (Optional)** | Streamlit / Flask |

---

### 🚀 Model Development
1. **Baseline Model:** Linear Regression (for trend analysis)  
2. **Advanced Models:** Random Forest & XGBoost (ensemble learning)  
3. **Hyperparameter Tuning:** GridSearchCV used for parameter optimization  
4. **Evaluation Metrics:** R² Score, MAE, MSE  

**Results Summary:**
| Model | R² | MAE | MSE |
|--------|----|-----|------|
| Linear Regression | -1.008 | 0.917 | 1.602 |
| Random Forest (Tuned) | **-0.987** | **0.893** | **1.585** |
| XGBoost (Tuned) | -1.147 | 0.952 | 1.712 |

✅ **Best Model:** RandomForest (Tuned)

---

### 🗺️ Geospatial Visualization
- Created **EV density heatmaps** using GeoPandas.  
- Computed **centroids** and **buffer coverage zones** using Shapely to highlight regions that require more stations.  
- Total combined coverage zone ≈ **7.83°²**, representing potential deployment regions.  

---

### 💡 Key Insights
- States like **Delhi**, **Karnataka**, and **Maharashtra** need more EV charging infrastructure.  
- **Southern and Western India** show higher EV adoption rates.  
- The framework can guide policymakers and planners for sustainable EV expansion.  


