# Diamond Price Prediction 2024
![Diamond](https://www.facebook.com/photo/?fbid=25347880224857549&set=gm.1120179732534161&idorvanity=1080575863161215)

This project involves predicting the prices of diamonds using machine learning models, specifically Random Forest and Decision Tree regressors. 
The dataset used for this project is sourced from Kaggle's "Diamond Price Prediction 2024" competition.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Models and Evaluation](#models-and-evaluation)
- [Contributing](#contributing)

## Project Overview

The goal of this project is to build predictive models that can accurately estimate the price of diamonds based on various attributes such as carat, cut, color, clarity, and dimensions. Two machine learning models are implemented and evaluated: Random Forest Regressor and Decision Tree Regressor.

## Dataset

The dataset used in this project is the "[Diamond Price Prediction 2024](https://www.kaggle.com/competitions/diamond-price-prediciton-2024/data)" dataset from Kaggle. It includes various features of diamonds and their corresponding prices.

- `carat`: The weight of the diamond.
- `cut`: The quality of the cut (Fair, Good, Very Good, Premium, Ideal).
- `color`: The diamond color, from D (best) to J (worst).
- `clarity`: A measurement of how clear the diamond is (IF, VVS1, VVS2, VS1, VS2, SI1, SI2, I1).
- `depth`: The total depth percentage.
- `table`: The width of the top of the diamond relative to the widest point.
- `price`: The price of the diamond.
- `x`: Length in mm.
- `y`: Width in mm.
- `z`: Depth in mm.

## Installation

To run the code in this repository, you need to have Python installed along with the necessary packages. You can install the required packages using pip:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```
## Usage
- Clone this repository to your local machine.
- Download the dataset from Kaggle and place it in the appropriate directory.
- Run the Jupyter notebook or Python scripts provided to train the models and make predictions.

## Models and Evaluation
### Data Preprocessing
- Log Transformation: Applied to numeric features to handle skewness.
- Label Encoding: Applied to categorical features (cut, color, clarity).
- Outlier Removal: Outliers were identified and removed using the IQR method.
- Feature Scaling: Standardization was applied to scale features.

### Random Forest Regressor
#### Hyperparameters:
- n_estimators: Number of trees in the forest.
- max_depth: Maximum depth of the tree.
- min_samples_split: Minimum number of samples required to split an internal node.
- min_samples_leaf: Minimum number of samples required to be at a leaf node.
- max_features: The number of features to consider when looking for the best split.

### Decision Tree Regressor
#### Hyperparameters:
- max_depth: Maximum depth of the tree.
- min_samples_split: Minimum number of samples required to split an internal node.
- min_samples_leaf: Minimum number of samples required to be at a leaf node.

### Evaluation Metrics
- RMSE: Root Mean Squared Error
- MAE: Mean Absolute Error
- MSE: Mean Squared Error
- R² Score: Coefficient of Determination

## Contributing
Contributions are welcome! Please fork this repository and submit a pull request for any improvements or bug fixes.
