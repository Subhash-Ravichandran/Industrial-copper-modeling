# Industrial Copper Modeling

## Problem Statement:
The copper industry grapples with data quality issues in sales and pricing, often leading to inaccuracies in manual predictions. Additionally, lead acquisition poses challenges in identifying high-potential prospects. This project aims to address these issues by implementing machine learning regression and classification models, alongside creating an interactive Streamlit application for efficient data input and prediction.

## Solution Overview:
1. **Data Preprocessing**: 
   - Handle missing values using mean/median/mode.
   - Treat outliers using IQR or Isolation Forest.
   - Address skewness in continuous variables with appropriate transformations.
   - Encode categorical variables using suitable techniques.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize outliers and skewness using Seaborn's plotting functions.
   - Feature engineering to create informative representations of the data.
   - Drop highly correlated columns.

3. **Model Building and Evaluation**:
   - Split dataset into training and testing/validation sets.
   - Train and evaluate classification models like ExtraTreesClassifier, XGBClassifier, or Logistic Regression.
   - Optimize model hyperparameters using cross-validation and grid search.

4. **Model GUI with Streamlit**:
   - Create an interactive Streamlit page.
   - Input task type (Regression or Classification).
   - Enter each column value (except 'Selling_Price' for regression and except 'Status' for classification).
   - Implement feature engineering, scaling, and transformation steps used during model training.
   - Predict and display output.

## Approach:
1. **Data Understanding**:
   - Identify variable types and distributions.
   - Treat rubbish values in 'Material_Reference'.
   - Drop 'INDEX' column if not useful.

2. **Data Preprocessing**:
   - Handle missing values, outliers, and skewness.
   - Encode categorical variables.
   
3. **EDA and Feature Engineering**:
   - Visualize outliers and skewness.
   - Engineer new features if applicable.
   - Drop highly correlated columns.
   
4. **Model Building and Evaluation**:
   - Train and evaluate classification and regression models.
   - Optimize model hyperparameters.
   
5. **Model GUI with Streamlit**:
   - Create an interactive page for input and prediction.
   - Implement feature engineering and transformation steps.
   - Use pickle module to load and use trained models.

## Usage:
1. Clone the repository.
2. Install required dependencies (`requirements.txt`).
3. Run the Streamlit application using `streamlit run app.py`.

## Tips:
- Use pickle module to dump and load models, encoders, and scaling factors.
- Fit and transform data separately for training and unseen data.

## Contributors:
- [Your Name]

## License:
[License Name and Link]
