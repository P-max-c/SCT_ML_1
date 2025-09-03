# House Prices Prediction with Random Forest

This project uses the **Kaggle House Prices: Advanced Regression Techniques** dataset to predict house sale prices.  
The workflow includes preprocessing, outlier removal, feature scaling, Random Forest regression, cross-validation, and visualization.

---

## Dataset
- **Train data**: `train.csv`  
- **Test data**: `test.csv`  
Both files come from [Kaggle House Prices competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).

---

## Steps
1. **Load Data**: Import training and test CSVs.  
2. **Preprocess**:  
   - Encode categorical columns with one-hot encoding.  
   - Remove outliers using Z-score.  
   - Handle missing values with median imputation.  
3. **Feature Scaling**: Standardize numerical features with `StandardScaler`.  
4. **Model Training**: Train a `RandomForestRegressor` with 100 trees.  
5. **Evaluation**:  
   - Perform 5-fold cross-validation.  
   - Report RMSE score.  
6. **Prediction**: Generate predictions on the test dataset.  
7. **Submission File**: Save results to `savesub.csv`.

---

## Visualizations
The project includes several plots for analysis:
- **Actual vs Predicted Prices** (training set scatter plot).  
- **Top 15 Feature Importances** (bar chart).  
- **Cross-Validation RMSE Distribution** (boxplot).  
- **Predicted Sale Price Distribution** (histogram).  

---

## Requirements
Install dependencies with:
```bash
pip install pandas numpy scikit-learn scipy matplotlib seaborn
