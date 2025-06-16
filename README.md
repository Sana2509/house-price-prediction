# house-price-prediction
predicting house prices using regression models and feature engineering
#  House Price Prediction

##  Project Summary

This project predicts house prices based on key features like **number of bedrooms**, **postcode**, **property type**, and **year of sale**. I built and compared multiple regression models and used **Random Forest Regressor** to achieve high prediction accuracy.

>  Final Model R² Score: **0.702**  
>  RMSE: **₹141,851.55**

---

##  Problem Statement

Real estate agents want to estimate housing prices using past sales data. The aim is to create a machine learning model that can **predict the selling price** of a property based on specific characteristics.

---

## 🧾 Features Used

| Feature        | Type        | Description                             |
|----------------|-------------|-----------------------------------------|
| `bedrooms`      | Numerical   | Number of bedrooms in the property      |
| `propertyType`  | Categorical | Type of property (e.g., House or Unit)  |
| `postcode`      | Categorical | Area code representing location         |
| `yearsold`      | Numerical   | Year extracted from `datesold` column   |

 **Target Variable**: `price` (log-transformed to reduce skew)

---

##  EDA Insights

- `price` is **right-skewed**, so log transformation was applied.
- More bedrooms = higher price (positive trend).
- **Houses** tend to sell at **higher prices** than units.
- Property prices increased over years → added `yearSold` feature.

##  Models Compared

| Model              | R² Score | RMSE (₹)      |
|--------------------|----------|---------------|
| Linear Regression  | 0.662    | ₹151,237.28   |
| **Random Forest**  | **0.702**| **₹141,851.55** |

Final model: **Random Forest Regressor** due to better performance.


## ⚙️ Tools & Technologies

- **Language**: Python
- **Libraries**:
  - Pandas, NumPy
  - Matplotlib, Seaborn
  - Scikit-learn (Pipeline, Preprocessing, Models)
- **IDE**: Jupyter Notebook

