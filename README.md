# deep-learning-challenge Analysis

## Purpose
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. The purpose of the analysis is to use deep learning to predict whether applicatants will be successful if funded by Alphabet Soup.

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
    * I am not able to reach the target performance: The model only has an accuracy of 0.7306 and a loss of 0.55, as the following image shows: ![main performance info](./Resources/main_performance.png)
    * I attempted to change the number of nodes and layers, and change the activation functions, but none of them seem to improve the model performace, and the optimized model has the following performance: ![optimization performance info](./Resources/optimization_performance.png)

## Summary
My models, before and after optimization, were only able to achieve around 73% accuracy and 0.55 loss. I also found out that adding too many layers might hurt the performance. Therefore, in order to solve this problem, I think we need to find the most optimal number of nodes and layers as well as the best activation function for this specific dataset.