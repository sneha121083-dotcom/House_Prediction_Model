# House Price Prediction Using Linear Regression

## Project Overview

This project implements a Machine Learning model to predict house prices using **Linear Regression**. It uses housing features such as overall quality, living area, garage capacity, basement area, number of bathrooms, and construction year to estimate the selling price of a house.

The project uses the Kaggle House Prices dataset and compares two Linear Regression models with different feature selections to evaluate predictive performance.

## Objectives

- Understand and analyze the housing dataset.
- Perform data cleaning and preprocessing.
- Explore relationships between housing features and selling prices.
- Train Linear Regression models.
- Predict house prices using selected features.
- Evaluate model performance using R² Score, MAE, and MSE.
- Visualize actual versus predicted house prices.

## Dataset

**Source:** [Kaggle – House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)

The dataset contains information about residential properties, including:

- Overall Quality
- Above-ground Living Area
- Number of Bedrooms
- Number of Bathrooms
- Garage Capacity
- Basement Area
- Year Built
- Year Remodeled
- Sale Price (Target Variable)

**Target Variable:** `SalePrice`

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## Project Workflow

1. Dataset collection and loading
2. Data exploration and statistical analysis
3. Handling missing values
4. Categorical feature encoding using One-Hot Encoding
5. Exploratory Data Analysis (EDA)
6. Correlation analysis and heatmap visualization
7. Feature selection
8. Train-test split (80:20)
9. Linear Regression model training
10. House price prediction
11. Model evaluation
12. Actual vs Predicted visualization
13. Model comparison and selection

## Machine Learning Models

Two Linear Regression models were developed.

**Model 1 – Baseline Model**

Uses five features:
- OverallQual
- GrLivArea
- BedroomAbvGr
- FullBath
- GarageCars

**Model 2 – Improved Model**

Uses seven features:
- OverallQual
- GrLivArea
- GarageCars
- TotalBsmtSF
- FullBath
- YearBuilt
- YearRemodAdd

## Model Evaluation Results

The models were evaluated using R² Score, Mean Absolute Error (MAE), and Mean Squared Error (MSE).

| Evaluation Metric | Model 1 | Model 2 |
|---|---:|---:|
| R² Score | 0.7719 | **0.7954** |
| MAE | 27,814.54 | **25,155.94** |
| MSE | 1.750 × 10⁹ | **1.569 × 10⁹** |

**Final Model Selected:** Model 2 – Linear Regression

Model 2 achieved an R² score of approximately **79.54%**, outperforming Model 1 across all three evaluation metrics on the test dataset.

## Visualizations

The project includes:

- Sale Price Distribution
- Correlation Heatmap
- Actual vs Predicted House Prices

These visualizations help understand feature relationships and evaluate prediction performance.

## How to Run the Project

1. Clone or download this repository.
2. Download the dataset from Kaggle.
3. Open the Jupyter Notebook in Google Colab.
4. Upload the `train.csv` dataset.
5. Execute the notebook cells sequentially.
6. Review the model evaluation results and visualizations.

## Future Improvements

- Experiment with additional relevant features.
- Apply feature scaling and advanced preprocessing pipelines.
- Handle outliers and skewed numerical features.
- Compare Linear Regression with Random Forest and Gradient Boosting.
- Perform hyperparameter tuning and cross-validation.
- Develop a simple web application for interactive house price prediction.

## Conclusion

This project demonstrates the application of supervised Machine Learning for house price prediction using Linear Regression.

By comparing two models with different feature selections, the improved model achieved an R² score of 79.54%. The project provided practical experience in data preprocessing, exploratory data analysis, feature selection, model training, prediction, and performance evaluation.

---

**Project Category:** Machine Learning | Regression

**Algorithm:** Linear Regression

**Dataset:** Kaggle – House Prices: Advanced Regression Techniques
