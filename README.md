# Water Quality Prediction

## Overview
This repository contains code for a machine learning model that predicts water quality based on various water quality parameters. It also includes data preprocessing, feature engineering, and model training using TensorFlow and Keras.

## Dataset
The dataset used for this project is "Water Quality Prediction.csv." It includes water quality measurements such as pH, iron content, nitrate levels, chloride concentration, and more.

## Data Preprocessing
- Initial data exploration and analysis are performed.
- Data is cleaned by removing rows with missing values.
- Numeric features are scaled to the range of [0, 1] using Min-Max scaling.
- Categorical features are one-hot encoded to convert them into a numeric format.
- The target variable is balanced using the Synthetic Minority Over-sampling Technique (SMOTE).

## Model
A neural network model is built using TensorFlow and Keras with the following layers:
- Input layer with 44 neurons (corresponding to the features).
- Three dense layers with ReLU activation functions (100, 200, and 100 neurons, respectively).
- Two dropout layers (40% dropout rate) to prevent overfitting.
- Output layer with a single neuron and sigmoid activation function.

The model is compiled with binary cross-entropy loss and stochastic gradient descent (SGD) optimizer.

## Training
The model is trained on the preprocessed data for 10 epochs.

## Evaluation
The trained model is evaluated on a test dataset, and the accuracy is calculated.

## Usage
You can use this code to predict water quality based on your own dataset. Make sure to install the required libraries and modify the code as needed.

## Dependencies
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Imbalanced-learn (for SMOTE)

## Author
Gunjit Bishnoi
