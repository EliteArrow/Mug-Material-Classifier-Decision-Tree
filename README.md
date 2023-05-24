# Mug Material Classifier(Decision Tree)

This Python project implements a Decision Tree classifier to predict the type of a material based on four measurements: height, diameter, weight, and hue. The problem is a multiclass classification problem, where the objective is to correctly predict one of three potential material types.

## Overview

1. **Data Loading**: The script loads a training set and a test set from CSV files.
2. **Data Preparation**: The script separates the features (measurements) from the labels (material types) in both the training and the test set.
3. **Model Training and Evaluation**: The Decision Tree model is trained and evaluated for varying depths, and the training and test accuracies are calculated and stored.
4. **Overfitting Analysis**: The model's performance at different tree depths is analyzed to identify potential overfitting.

## Data

The data directory should contain two csv files:

- `data_train.csv`: The training data, including given columns

| Height | Diameter | Weight | Hue | Type |
| --- | --- | --- | --- | --- |
- `data_test.csv`: The test data, including given columns

| Height | Diameter | Weight | Hue | Type |
| --- | --- | --- | --- | --- |

## Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- scikit-learn
- collections

## Results

The script prints the test predictions for the maximum pure depth of the Decision Tree. It then trains and tests the model for varying tree depths from 1 to 8, and outputs the accuracy for both the training and testing datasets. The results are also visualized in a plot, showing how accuracy changes with tree depth.

The script concludes by printing the depths at which the model is overfitting, as evidenced by a high training accuracy and lower test accuracy.

## Optional

The decision tree model is also visualized using `sklearn.tree.plot_tree`. This requires the sklearn library. The decision tree is plotted with nodes filled with colors corresponding to classes, feature names are shown on branches, and class names are shown at leaf nodes.

**Note**: This is an optional section and can be commented out if not needed.
