# 🔍 Customer Churn Prediction (Machine Learning)

## 💡 How To Install
```bash
1. Copy the repo link
2. Run: git clone [repo-link]
```

## 🛠️ Requirements Installation
```bash
pip install -r requirements.txt
```
*Required libraries:*
- pandas
- numpy
- matplotlib
- scikit-learn

## 🔍 About the Project
This project builds a machine learning model to predict customer churn for a telecommunications company. It analyzes customer data to identify patterns and predict whether a customer is likely to leave the service.

### 📊 Features
🔧 **Data Preprocessing**
- Handles missing values and non-numeric data (e.g., converting empty strings in `TotalCharges` to NaN)
- Encodes categorical variables using `LabelEncoder` for model compatibility
- Checks for data integrity (e.g., no missing values in the dataset)

📈 **Dataset Overview**
- Contains 7,043 customer records with 21 features, including:
  - Demographic info (`gender`, `SeniorCitizen`, `Partner`, `Dependents`)
  - Service details (`PhoneService`, `InternetService`, `OnlineSecurity`, etc.)
  - Billing info (`MonthlyCharges`, `TotalCharges`, `PaymentMethod`)
  - Target variable: `Churn` (Yes/No)
- No missing values in the dataset
- `TotalCharges` required cleaning due to non-numeric entries (e.g., spaces)

🔍 **Exploratory Data Analysis (EDA)**
- Displays unique values for each feature to understand data distribution
- Provides descriptive statistics for numerical features (`tenure`, `MonthlyCharges`, `SeniorCitizen`)
- Identifies and resolves data type issues (e.g., `TotalCharges` as object)

🛡️ **Data Preparation**
- Converts categorical variables (e.g., `gender`, `Contract`, `Churn`) to numerical values
- Ensures all features are in a suitable format for machine learning models

### ✨ Project Benefits
- **Actionable Insights**: Helps businesses identify at-risk customers and implement retention strategies
- **Clean Data Pipeline**: Robust preprocessing ensures reliable model input
- **Scalable Foundation**: Easily extendable for model training and evaluation
- **User-Friendly**: Well-documented Jupyter notebook for easy exploration and modification

## 🚀 Next Steps
- Split the dataset into training and testing sets
- Train machine learning models (e.g., Logistic Regression, Random Forest, XGBoost)
- Evaluate model performance using metrics like accuracy, precision, recall, and F1-score
- Visualize feature importance to understand key drivers of churn

## 📝 Notes
- The notebook currently focuses on data preprocessing and EDA. Model training and evaluation steps are not included but can be added.
- Ensure the dataset file (`Customer_Churn_dataset.csv`) is in the correct directory before running the notebook.
- The `TotalCharges` column contains some non-numeric values (spaces), which are handled by converting them to NaN.

### Instructions for Use
1. Clone the repository and install the required libraries.
2. Place the `Customer_Churn_dataset.csv` file in the appropriate directory (e.g., `D:\Development\Python Projects\Machine Learning\Microsoft\`).
3. Open the `Customer_churn_ML_model.ipynb` notebook in Jupyter or a compatible environment.
4. Run the cells sequentially to preprocess the data and explore the dataset.
5. Extend the notebook with model training and evaluation as needed.