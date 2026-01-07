# 🛰️ Satellite Imagery Based Property Valuation

This project predicts **house prices using both tabular data and satellite imagery**.  
It combines traditional house attributes with **visual information from satellite images** using deep learning and gradient boosting.

---

## 📌 Project Pipeline

The project is organized into **three main steps**:

1. **Data Fetcher**  
   Downloads satellite images using latitude and longitude from the dataset.

2. **Preprocessing**  
   - Extracts handcrafted visual features (green cover %, urban density %)  
   - Extracts deep features from images using ResNet18 CNN  
   - Merges tabular + visual + CNN features into final datasets

3. **Model Training**  
   - Applies scaling and PCA on CNN features  
   - Trains XGBoost regression model  
   - Evaluates performance  
   - Predicts prices for test set

---
