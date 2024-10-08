# Business Understanding

In the rapidly growing real estate market, accurate house price predictions are crucial. The real estate industry faces the critical task of determining appropriate pricing for houses by analyzing factors such as location, size, amenities, and market trends. Effective price predictions provide valuable insights to investors, buyers, and real estate professionals, enabling informed decision-making and improved investment strategies

# Porject Objective
- The goal of this project is to predict house prices using the Pakistan House 2023.
- The dataset contains eight columns, with house price as the dependent variable and seven other features as independent variables. [Access the Dataset here](https://www.kaggle.com/datasets/manjitbaishya001/house-prices-2023)


- A linear regression model was implemented using PySpark's machine learning library to predict house prices.
- Evaluation metrics, such as MAE, RMSE, and MSE, were used to assess the model's performance on both the training and test datasets.
  
# Project Overview : 
This project involved several key steps to predict house prices using the Pakistan House 2023 dataset:
- **Data Import and Initialization**: Set up Spark for local execution and imported necessary libraries such as NumPy, Matplotlib, and PySpark.
- **Data Pre-Processing**
  - **Data Cleaning**:  Removed unnecessary characters and converted string columns into appropriate integer types.
  - **Handling Missing and Inconsistent Data**: Applied the dropna method to remove rows with missing values and ensured consistent data across relevant columns.
  - **Feature Encoding**: Transformed categorical variables (e.g., property type, city, and purpose) into numerical form using StringIndexer and OneHotEncoder.
- **Handling Outlier**: Applied the Interquartile Range (IQR) method to detect and remove outliers in continuous variables.
- **Standard Scaller**: Scaled the feature set using StandardScaler to normalize features, ensuring that each feature contributes equally to model training.
- **Train-Test Split**: Divided the dataset into 70% for training and 30% for testing to evaluate model performance on unseen data.
- **Building Model and Evaluation**
  - Building a linear regression model using PySpark.
  - Evaluated performance using metrics such as MAE, RMSE, and MSE for both training and test data.
  - Visualized predicted vs. actual prices, showing a linear relationship with some prediction errors.

# Project Result
- The linear regression model exhibited a positive correlation between actual and predicted house prices for both training and test datasets.
- Evaluation metrics (MAE, RMSE, and MSE) showed similar error values for both training and test sets, reflecting consistent model performance, though the error magnitudes indicate significant deviations from actual prices.
- Although the model demonstrated a linear relationship between actual and predicted prices, the relatively high error values highlight potential limitations, possibly due to feature insufficiency or model complexity.

# Conclusion
The project successfully applied PySpark to predict house prices. Despite a clear linear relationship, high error values suggest further improvements are needed, such as refining feature selection and model complexity for better accuracy in future predictions.
