# ML_Project
# 🫐 Wild Blueberry Yield Prediction with Random Forest

A machine learning project predicting the **yield** of wild blueberries using features like pollinator activity, temperature ranges, and rainfall patterns. The model was trained and tuned using **Random Forest Regression** with hyperparameter tuning & feature importance visualization.

## 🔍 Dataset Info

- **Source**: `WildBlueberryPollinationSimulationData.csv`
- **Rows**: 777  
- **Columns**: 17 (after dropping `Row#`)
- **Target**: `yield`

## 📊 EDA Highlights

- Explored correlations, skewness, boxplots & histograms.
- Top features positively correlated with yield:  
  `fruitset`, `seeds`, `fruitmass`, `osmia`  
- Features negatively correlated:  
  `AverageRainingDays`, `RainingDays`, `clonesize`

## ⚙️ Model Used

- **Base**: RandomForestRegressor
- **Tuned With**: GridSearchCV
- **Best Parameters**:
  ```python
  {
    'n_estimators': 200,
    'max_depth': 12,
    'min_samples_split': 2,
    'min_samples_leaf': 1,
    'max_features': 'sqrt'
  }
## Shoutout

Special Thanks to **GenEd-Tech** for the sessions and support throughout the course.  
Appreciate the solid teaching. ✨
