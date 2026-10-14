# Task 3: Car Price Prediction with Machine Learning

## 📌 Project Overview

This project focuses on building a Machine Learning regression model to predict the selling price of used cars based on features such as car brand, age, mileage, fuel type, transmission, and other relevant vehicle characteristics.

The project follows a complete Machine Learning workflow, including data cleaning, feature engineering, exploratory data analysis (EDA), categorical encoding, model training, and performance evaluation.

Multiple regression algorithms are trained and compared to identify the best-performing model for predicting used car prices.

## 🎯 Objectives

- Clean and preprocess the used-car dataset.
- Handle missing values, duplicate records, and inconsistent categorical values.
- Engineer new features, including car age and car brand.
- Explore relationships between selling prices and vehicle characteristics.
- Visualize price distributions and correlations between numerical features.
- Encode categorical variables for Machine Learning.
- Train and compare at least two regression models.
- Evaluate model performance using MAE, RMSE, and R².
- Identify the most influential features using a feature importance chart.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning:** Scikit-learn
- **Data Visualization:** Matplotlib, Seaborn
- **Development Environment:** Jupyter Notebook

## 📂 Project Structure

```text
OIBSIP/
└── Data Science/
    └── Task-3-Car-Price-Prediction/
        ├── README.md
        ├── Car_Price_Prediction_with_Machine_Learning.ipynb
        └── data/
            └── car_data.csv
```

*Note: Update the folder structure and dataset filename to match your actual project files.*

## 📊 Dataset

The project uses a dataset containing information about used cars and their selling prices.

Depending on the selected dataset, features may include:

- **Car_Name:** Name or model of the car.
- **Year:** Year of manufacture.
- **Selling_Price:** Selling price of the used car (target variable).
- **Present_Price:** Current market price or reference price, if available.
- **Kms_Driven:** Distance travelled by the car.
- **Fuel_Type:** Fuel type, such as Petrol, Diesel, or CNG.
- **Seller_Type:** Individual or dealer.
- **Transmission:** Manual or Automatic.
- **Owner:** Number of previous owners, if available.

The exact columns depend on the dataset selected for the project.

## 🔍 Project Workflow

### 1. Data Loading and Inspection

- Load the dataset using Pandas.
- Inspect the dataset's shape and column names.
- Examine data types and summary statistics.
- Identify missing values and duplicate records.
- Check for inconsistent categorical values.

### 2. Data Cleaning and Preprocessing

- Handle missing values appropriately.
- Remove duplicate records where necessary.
- Standardize categorical values, such as `Petrol` and `petrol`.
- Check for invalid values and potential outliers.
- Prepare the dataset for exploratory analysis and model training.

### 3. Feature Engineering

- Calculate **Car Age** using the year of manufacture and a defined reference year.
- Extract the **Brand** from the car name.
- Select relevant features for predicting the selling price.
- Exclude identifiers or irrelevant columns where appropriate.

### 4. Exploratory Data Analysis (EDA)

The analysis includes:

- **Selling Price Distribution:** Understand the distribution and spread of used-car prices.
- **Price vs. Fuel Type:** Compare selling prices across fuel categories using box plots.
- **Price vs. Car Age:** Examine how vehicle age relates to selling price using a scatter plot.
- **Feature Correlation Heatmap:** Investigate relationships between numerical features.
- **Additional Visualizations:** Explore the effects of mileage, transmission, brand, and other variables where available.

### 5. Feature Encoding

Categorical variables are converted into numerical representations using an appropriate encoding technique, such as One-Hot Encoding.

The preprocessing workflow is designed to ensure that training and test data are handled consistently.

### 6. Model Training

The dataset is divided into training and testing sets to evaluate performance on unseen data.

At least two regression algorithms are trained and compared, such as:

- **Linear Regression:** A baseline model for learning linear relationships between features and selling price.
- **Random Forest Regressor:** An ensemble model capable of capturing nonlinear relationships.
- **Gradient Boosting Regressor:** An optional additional model for comparison.

The final model selection is based on evaluation results rather than assumptions about which algorithm performs best.

### 7. Model Evaluation

The models are evaluated using three regression metrics:

- **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted prices.
- **Root Mean Squared Error (RMSE):** Penalizes larger prediction errors more heavily.
- **R² Score:** Measures how well the model explains variation in the target variable.

Lower MAE and RMSE values generally indicate better predictions, while a higher R² score generally indicates a better fit.

### 8. Feature Importance

A feature importance chart is created for the selected best-performing model, where supported by the chosen algorithm.

This visualization helps identify which vehicle characteristics contribute most to the model's predictions.

## ⚙️ Installation and Setup

### Prerequisites

Install Python 3.9 or later and Jupyter Notebook.

### Install Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### Run the Project

1. Clone or download the repository.
2. Place the dataset in the project directory.
3. Open a terminal in the project folder.
4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `car_price_prediction.ipynb`.
6. Update the dataset path if necessary.
7. Run all notebook cells in sequence.

## 📈 Expected Outcomes

- A cleaned and analysis-ready used-car dataset.
- Visual insights into selling prices and vehicle characteristics.
- Engineered features representing car age and brand.
- At least two trained regression models.
- A comparison of model performance using MAE, RMSE, and R².
- A feature importance visualization for the selected model.
- Identification of a suitable regression model for used-car price prediction.

## ⚠️ Limitations

Model performance depends on dataset quality, feature selection, and the range of vehicles represented in the data.

Predictions may be less reliable for vehicles that differ significantly from the training data. Feature importance indicates predictive contribution, not necessarily a causal relationship.

Care should also be taken to avoid data leakage by excluding information that would not realistically be available when making a prediction.

## 👨‍💻 Author

**Hazem Ebrahim**

Data Science Intern | Python | Data Analysis | Machine Learning

## 📜 Acknowledgment

This project is completed as part of **Task 3: Car Price Prediction with Machine Learning** under the Oasis Infobyte Internship Program (OIBSIP).

---

*If you find this project useful, feel free to star the repository.*
