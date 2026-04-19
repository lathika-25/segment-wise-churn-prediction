# Customer Churn Prediction (Segment-wise Approach)

Machine learning project using XGBoost to predict customer churn with behavioral data analysis.

## Project Overview
This project predicts customer churn using a segment-wise machine learning approach. Instead of using a single model, customers are divided based on tenure and separate models are trained for each segment to improve prediction accuracy and business insights.

---

## Objective
- Predict customer churn using machine learning
- Compare baseline vs segment-wise models
- Improve performance by analyzing different customer groups

---

## Dataset
- Telco Customer Churn Dataset  
- 7043 customer records  
- Features include demographics, services, billing, and customer behavior  

---

## Project Workflow

### 1. Data Preprocessing
- Removed duplicates and handled missing values  
- Dropped irrelevant columns (CustomerID, location fields)  
- Eliminated data leakage columns (ChurnScore, ChurnCategory, ChurnReason, CustomerStatus)  

### 2. Feature Engineering
- Applied One-Hot Encoding for categorical variables  
- Converted target variable (ChurnLabel) to numeric  

### 3. Model Building
- Baseline: Logistic Regression  
- Segment-wise models based on tenure  
- XGBoost for improved performance  

### 4. Segmentation Strategy

| Segment | Tenure |
|--------|--------|
| New    | ≤ 12 months |
| Mid    | 13–36 months |
| Long   | > 36 months |

---

## Results
- Baseline accuracy: ~94%  
- Segment-wise models provided better insights into customer behavior and churn patterns  

---

## Key Learnings
- Importance of data preprocessing and cleaning  
- Impact of data leakage on model performance  
- Benefits of segment-wise modeling  
- Handling high-dimensional encoded data  

---

## Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  
- Google Colab  

---

## Future Improvements
- Hyperparameter tuning  
- Advanced models (Random Forest, XGBoost optimization)  
- Dashboard visualization (Streamlit / Power BI)  
- Deployment as a web application  

---

## Author
Lathikeswari Ramanathan
