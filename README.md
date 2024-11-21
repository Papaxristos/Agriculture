# Wheat Production Prediction using Gradient Boosting

This project uses machine learning to predict wheat production based on historical data. The model utilizes the Gradient Boosting Regressor algorithm to make predictions, and the process includes several key steps, from data cleaning to model optimization.

## Project Overview

The goal of this project is to predict the wheat production in tonnes for various years based on input features. The dataset is cleaned and preprocessed, with missing values handled and categorical variables encoded into numerical format. The model is built using Gradient Boosting, and optimization techniques are applied to improve its performance.

## Dataset

The dataset used in this project is `wheat-production.csv`, which contains the wheat production data along with various features that influence production.

### Columns:
- **Year**: The year of the production record.
- **Production**: The wheat production in tonnes.
- *(Additional columns based on the dataset's content)*

## Steps Taken in the Project

### 1. Data Loading
- The data is loaded from a CSV file located in Google Drive.

### 2. Data Preprocessing
- Missing values in numeric columns are replaced by the mean of each column.
- Categorical columns are encoded into numerical values using `LabelEncoder`.

### 3. Data Exploration
- Basic statistical analysis is performed to examine the dataset.
- Visualizations such as histograms, pairplots, and heatmaps are created to explore the relationships and distributions in the data.

### 4. Outlier Detection and Removal
- Outliers are detected using the Z-score method and removed to improve the model's accuracy.

### 5. Model Building and Training
- A Gradient Boosting Regressor model is used for prediction.
- The model is optimized by adjusting the hyperparameters such as the number of estimators and the learning rate.

### 6. Model Evaluation
- The performance of both the initial and optimized models is evaluated using metrics such as Mean Squared Error (MSE) and R-squared (R²).
- Visualizations are created to compare the actual and predicted values.

### 7. Results
- The results, including the actual and predicted wheat production values, are saved to a new CSV file.
- A scatter plot is created to visualize the relationship between the actual and predicted values.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/wheat-production-prediction.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Upload the `wheat-production.csv` dataset to your Google Drive.
2. Run the `wheat_production_prediction.py` script in Google Colab or your local environment.
3. The results will be saved in a new CSV file `wheat_predictions.csv` in your Google Drive.

## Dependencies

- `numpy`
- `pandas`
- `seaborn`
- `scipy`
- `matplotlib`
- `xgboost`
- `sklearn`

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Dataset from [source].
- Machine Learning algorithms from `scikit-learn` and `xgboost`.
