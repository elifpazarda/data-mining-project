# Contraceptive Method Choice Analysis

This project analyzes contraceptive method choices using machine learning classification models. The analysis aims to predict contraceptive method choices based on various demographic and socio-economic factors.

[Youtube Presentation](https://www.youtube.com/watch?v=NIunpuFBiFA)

## Dataset Description

The dataset contains information about contraceptive method choices and various demographic factors. Each record represents a married woman with the following attributes:

1. Wife's age (numerical)
2. Wife's education (categorical): 1=low, 2, 3, 4=high
3. Husband's education (categorical): 1=low, 2, 3, 4=high
4. Number of children ever born (numerical)
5. Wife's religion (binary): 0=Non-Islam, 1=Islam
6. Wife's now working? (binary): 0=Yes, 1=No
7. Husband's occupation (categorical): 1, 2, 3, 4
8. Standard-of-living index (categorical): 1=low, 2, 3, 4=high
9. Media exposure (binary): 0=Good, 1=Not good
10. Contraceptive method used (class attribute): 1=No-use, 2=Long-term, 3=Short-term

## Project Structure

- `trees.ipynb`: Jupyter notebook containing the complete analysis
- `dataset.csv`: Raw dataset file
- `README.md`: Project documentation

## Analysis Overview

The project implements and compares two machine learning models:
1. Decision Tree Classifier
2. Random Forest Classifier

The analysis includes:
- Data preprocessing and exploration
- Feature correlation analysis
- Model training and hyperparameter tuning using GridSearchCV
- Model evaluation using various metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC curves
  - Confusion matrices

## Key Findings

- Both models show moderate performance in predicting contraceptive method choices
- Decision Tree Performance:
  - Accuracy: ~59%
  - Best performance in predicting "No-use" category (Class 1)
  
- Random Forest Performance:
  - Accuracy: ~56%
  - More balanced performance across classes
  - Better precision for "No-use" category

## Requirements

The project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Usage

1. Ensure all required libraries are installed
2. Run the Jupyter notebook `trees.ipynb`
3. The notebook contains detailed analysis with visualizations and model comparisons

## Model Evaluation

The models are evaluated using:
- 5-fold cross-validation
- Multiple performance metrics
- Visualization of results through:
  - Confusion matrices
  - ROC curves
  - Performance comparison plots
