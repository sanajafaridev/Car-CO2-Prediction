# Car CO₂ Emissions Prediction

## Overview

This project uses machine learning to predict vehicle CO₂ emissions based on vehicle-related features.

The project explores the dataset, visualizes relationships between features, trains regression models, and evaluates their performance using different metrics.

## Objectives

- Explore and analyze vehicle data.
- Visualize relationships between vehicle features and CO₂ emissions.
- Build and compare regression models.
- Evaluate model performance on unseen test data.
- Investigate potential overfitting in the Random Forest model.

## Technologies & Libraries

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Machine Learning Models

Two regression algorithms are used:

- **Linear Regression**
- **Random Forest Regressor**

The Random Forest model uses 100 trees and a fixed random state to make its results reproducible.

## Project Workflow

1. Load and explore the dataset.
2. Analyze the data using descriptive statistics and visualizations.
3. Separate the input features and target variable.
4. Split the data into training and testing sets.
5. Train both regression models.
6. Evaluate their performance using:
   - Mean Squared Error (MSE)
   - Mean Absolute Error (MAE)
   - R² Score
7. Experiment with different `max_depth` values for Random Forest.
8. Compare training and testing errors to investigate overfitting.
9. Visualize actual and predicted CO₂ emissions.

## Results

### Model Comparison

Both models are evaluated on the same training and testing split.

| Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MSE | 878.41 | 284.98 |
| MAE | 22.40 | 7.34 |
| R² Score | 0.85 | 0.95 |

On the evaluated test set, Random Forest achieved lower prediction errors and a higher R² score than Linear Regression.

### Overfitting Analysis

For the Random Forest model, the following Mean Squared Errors were observed:

- **Training MSE:** 41.46
- **Testing MSE:** 284.98

The difference between training and testing errors suggests potential overfitting. This highlights the importance of evaluating machine learning models on data they have not seen during training.

## Visualizations

The notebook includes visualizations for data exploration, feature relationships, and comparisons between actual and predicted CO₂ emissions.

## Dataset

The dataset is not included in this repository.

To run the notebook, obtain the required dataset separately and make sure it is available at the file path expected by the notebook.

The target variable is `out1`, and the input features are the remaining columns in the dataset.

## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Obtain the dataset separately.
4. Place the dataset in the appropriate location or update the file path in the notebook.
5. Open the Jupyter Notebook.
6. Run the cells in order.

## Future Improvements

- Use cross-validation for more robust model evaluation.
- Further investigate overfitting and model generalization.
- Experiment with additional model configurations.
- Improve visualizations and feature analysis.

## Learning Notes

This project was developed as part of my machine learning learning journey, with a focus on regression, model evaluation, and understanding the trade-off between training performance and generalization.