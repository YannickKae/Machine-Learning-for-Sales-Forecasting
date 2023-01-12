# Machine Learning for Sales Forecasting
This R Markdown script can be used for building a predictive model to forecast the sales of a bakery in Kiel, Germany. It is designed to be run in an R environment and makes use of several R and Python libraries. It loads and prepares a time-series dataset where each row represents a day and each column represents a feature.

The script performs the following operations:

1. Loads R libraries: "readr", "fastDummies", "reticulate", "ggplot2", "Metrics"
2. Recodes the "Wochentag" column into dummy variables
3. Selects the feature variables and the label variable from the dummy dataset.
4. Splits the dataset into training, validation, and test datasets.
5. Uses Tensorflow to construct a neural network model using the Sequential API.
6. The model uses Dense, BatchNormalization and Dropout layers, as well as an Adam optimizer for training.
7. The model is trained on the training dataset and can be used to make predictions about the sales on the next day.
