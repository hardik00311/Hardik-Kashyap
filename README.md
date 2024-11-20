# Crop Yield Prediction Using Machine Learning

## Project Overview
This project leverages machine learning techniques to predict crop yields across 101 countries and 10 major crops using various features such as rainfall, temperature, pesticide usage, country, and crop type. The *Decision Tree Regressor* demonstrated the best performance, making it a scalable and interpretable solution for agricultural decision-making.

## Objectives
•⁠  ⁠Develop a machine learning model for accurate crop yield prediction.
•⁠  ⁠Identify key factors influencing yield variability.
•⁠  ⁠Provide a scalable solution applicable across diverse regions and crops.

## Dataset
•⁠  ⁠*Countries*: 101
•⁠  ⁠*Crops*: 10 (e.g., wheat, maize, rice, etc.)
•⁠  ⁠*Features*:
  - Year
  - Rainfall (mm)
  - Temperature (°C)
  - Pesticide usage (kg/ha)
  - Country (categorical)
  - Crop type (categorical)
•⁠  ⁠*Target*: Crop yield (tons/ha)

## Methodology
1.⁠ ⁠*Data Preprocessing*
   - Missing values imputed with mean/median values.
   - Categorical features encoded using one-hot encoding.
   - Continuous variables normalized.

2.⁠ ⁠*Exploratory Data Analysis (EDA)*
   - Significant correlations observed between temperature, rainfall, and yield.
   - Pesticide usage correlated with diminishing yield improvements in some cases.

3.⁠ ⁠*Model Selection and Training*
   - Models evaluated: Linear Regression, Lasso, Ridge, Decision Tree.
   - Best model: *Decision Tree Regressor*.
   - Evaluation metrics: MAE, RMSE, R² Score.

4.⁠ ⁠*Validation*
   - Data split: 80% training, 20% testing.
   - 5-fold cross-validation applied.
   - Hyperparameter tuning for optimal performance.

## Results
| Model               | MAE  | RMSE  | R² Score | Accuracy |
|---------------------|-------|-------|----------|----------|
| Linear Regression   | 1.85 | 2.62  | 0.65     | 74.2%    |
| Lasso Regression    | 1.82 | 2.58  | 0.66     | 74.3%    |
| Ridge Regression    | 1.80 | 2.55  | 0.67     | 74.1%    |
| *Decision Tree*   | 1.10 | 1.72  | 0.89     | 98.0%    |

•⁠  ⁠*Key Predictors*: Rainfall, temperature, and pesticide usage.
•⁠  ⁠Countries with moderate climates exhibited more consistent yield predictions.

## Tools and Technologies
•⁠  ⁠*Programming*: Python
•⁠  ⁠*Libraries*: Pandas, NumPy, Scikit-learn, Matplotlib
•⁠  ⁠*Environment*: Google Colab

## Key Findings
•⁠  ⁠The Decision Tree Regressor excelled due to its ability to handle non-linear interactions.
•⁠  ⁠Rainfall and temperature were the most influential factors affecting crop yields.

## Limitations and Future Work
### Limitations
•⁠  ⁠Lack of features like soil quality and irrigation data.
•⁠  ⁠Dataset did not account for extreme weather events.

### Future Work
•⁠  ⁠Include additional data on soil quality and market conditions.
•⁠  ⁠Explore ensemble methods (e.g., Random Forest) for better generalization.

## References
•⁠  ⁠*Dataset Sources*:
  - [FAO](http://www.fao.org/home/en/)
  - [World Bank](https://data.worldbank.org/)
•⁠  ⁠*Libraries and Tools*:
  - [Scikit-learn](https://scikit-learn.org/)
  - [NumPy](https://numpy.org/)
  - [Pandas](https://pandas.pydata.org/)

---

### How to Run the Project
1.⁠ ⁠Clone this repository:
   ```bash
   git clone https://github.com/Hardik-Kashyap/ML_Project_Crop.ipynb
