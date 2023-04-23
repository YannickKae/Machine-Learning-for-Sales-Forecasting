# Sales Forecasting with Machine Learning

This repository provides an R Markdown script for building and training a predictive machine learning model to forecast daily sales of a bakery in Kiel, Germany. The script is designed to be run in an R environment and utilizes both R and Python libraries for data preprocessing and model training.

## Features

- Load and prepare a time-series dataset where each row represents a day and each column represents a feature
- Utilize R libraries: "readr", "fastDummies", "reticulate", "ggplot2", "Metrics"
- Perform data preprocessing, including recoding the "Wochentag" column into dummy variables
- Split the dataset into training, validation, and test datasets
- Construct a neural network model using TensorFlow and Keras
- Train the model on the training dataset and validate its performance
- Generate sales forecasts for future days

## Getting Started

1. Install the required R libraries:
```
install.packages(c("readr", "fastDummies", "reticulate", "ggplot2", "Metrics"))
```

2. Ensure you have Python and TensorFlow installed in your environment. You can install TensorFlow using the following command:
```
pip install tensorflow
```

3. Run the R Markdown script to preprocess the data, train the model, and make sales predictions.

## Model Architecture

The neural network model is constructed using the TensorFlow and Keras libraries. The model consists of:

- An InputLayer to specify the input shape
- BatchNormalization for data normalization
- Dense layers with ReLU activation functions for non-linear transformations
- Dropout layers for regularization to prevent overfitting
- An Adam optimizer for training

## Results

The script trains the model on the training dataset and evaluates its performance using the validation dataset. The model can then be used to make predictions about the sales for the next day. Visualizations are provided to compare the predicted and actual sales values for both the training and validation datasets.
