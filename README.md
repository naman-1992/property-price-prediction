[Mini_Project_Propery_Price_Predict.ipynb](https://github.com/user-attachments/files/24414157/Mini_Project_Propery_Price_Predict.ipynb)# Property Price Prediction (Mini Project)

##  Overview
This project aims to predict property sale prices using machine learning techniques. By analyzing housing features such as lot size, overall quality, year built, and garage details, the model provides insights into the factors that most influence property values.
The workflow includes:
- Exploratory Data Analysis (EDA)
- Data cleaning and handling missing values
- Feature engineering (log transformation, encoding categorical variables)
- Model training and evaluation (Linear Regression, Decision Tree, Random Forest)
- Business insights from feature importance

---

##  Tech Stack
- **Python**: NumPy, Pandas, Scikit-learn  
- **Visualization**: Matplotlib, Seaborn  
- **Models**: Linear Regression, Decision Tree Regressor, Random Forest Regressor  

---

##  Dataset
- Source: property_price_data.csv
- Size: 970 rows × 69 columns
- Target Variable: SalePrice (log-transformed as LogSalePrice)
- Key Features:
- OverallQual, GrLivArea, GarageCars, GarageArea, YearBuilt, TotalBsmtSF
- Neighborhood, zoning, and other categorical features


---

## Methodology
## Data Preprocessing.
  - Dropped high-null columns (MiscFeature, Alley, Fence, Prop_Id)
  - Filled missing numeric values with median, categorical with "None"
  - Applied log transformation to SalePrice to correct skewness
## Feature Engineering
  - One-hot encoding for categorical variables
  - Correlation analysis to identify top predictors
## Modeling
  - ## Linear Regression – baseline model
  - ## Decision Tree Regressor – non-linear splits
  - ## BRandom Forest Regressor – ensemble approach for improved accuracy
## Evaluation Metrics
  - ## Mean Absolute Error (MAE)
  - ## Mean Squared Error (MSE)
  - ## R² Score

Results
- Top Correlated Features with Sale Price:
- ## OverallQual (0.82)
- ## GrLivArea (0.69)
- ## GarageCars (0.68)
- ## GarageArea (0.65)
- ## YearBuilt (0.58)
- Model Performance (example placeholders, replace with your actual results):
  ## -------Model------    --MAE--    -RMSE-    -R2 score-
  ## -Linear Regression  -  25,000  - 40,000  -   0.72
  ## -Decision Tree      -  22,000  - 35,000  -   0.78
  ## -Random Forest      -  18,000  - 30,000  -   0.85

## 📈 Key Insights
- **Top Predictors**: `OverallQual`, `GrLivArea`, `GarageCars`, `YearBuilt`  
- **Random Forest** outperformed other models with higher accuracy and lower error.  
- Feature importance analysis provided actionable insights into property valuation.

---

[Mini_Project_Propery_Price_Predict.pdf](https://github.com/user-attachments/files/24414153/Mini_Project_Propery_Price_Predict.pdf)
Author

## Naman Singh Pathania
- Data Science & Machine Learning Enthusiast
- Focused on building interpretable models and actionable insights

git clone https://github.com/yourusername/property-price-predict.git
cd property-price-predict

pip install -r requirements.txt

jupyter notebook Mini_Project_Property_Price_Predict.ipynb

