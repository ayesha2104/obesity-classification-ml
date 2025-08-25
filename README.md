# Obesity Classification using Machine Learning

This project predicts obesity levels based on lifestyle, dietary habits, and physical attributes.  
Dataset: Combination of synthetic and real data collected from individuals in Mexico, Peru, and Colombia.  

## Project Workflow
1. **Data Preprocessing**
   - Converted categorical variables using Label Encoding
   - Handled outliers with Isolation Forest (removed 64 anomalies)
   - Scaled features with StandardScaler

2. **Exploratory Data Analysis**
   - Distribution plots, correlation heatmaps, and boxplots
   - Gender-wise obesity trends
   - Lifestyle impact on obesity levels

3. **Clustering**
   - Applied **DBSCAN** and **KMeans with LDA** for group discovery
   - Identified 4 lifestyle-obesity clusters

4. **Model Training**
   - Logistic Regression: 88.0% accuracy
   - Random Forest: 94.9% accuracy
   - SVM: 91.2% accuracy
   - KNN: 85.9% accuracy
   - **XGBoost: 96.3% accuracy (best model)**

5. **Explainability**
   - SHAP values to interpret feature importance
   - Key drivers: Weight, Gender, Diet, Physical activity, Hydration

## Results
- **Best Model**: XGBoost with 96% accuracy
- Strong class-wise performance across 7 obesity categories
- Insights can support **public health early-warning systems** and **personalized health programs**

## Repository Structure
- `notebooks/`: Jupyter notebook with full workflow
- `reports/`: Exported PDF & HTML versions
- `data/`: Dataset (if included)

## Future Work
- Use larger real-world datasets
- Track obesity progression with longitudinal data
- Integrate deep learning for feature extraction
