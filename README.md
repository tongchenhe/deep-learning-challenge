# deep-learning-challenge Analysis

## Purpose
The purpose of the analysis is to use deep learning to predict whether applicatants will be successful if funded by Alphabet Soup.

## Results
* Data Preprocessing:
    * Our target variable is the `IS_SUCCESSFUL` column
    * The features for our model are `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`
    * The `EIN` and `NAME` columns were removed because they are identification variables.

* Compiling, Training, and Evaluating the Model
    * My initial model includes:
        * The first layer with 8 nodes and activation function sigmoid
        * The second layer with 8 nodes and activation function tanh
        * An output layer with activation function relu
