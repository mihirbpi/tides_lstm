# tides_lstm
Predicting SF water levels using LSTMs in TensorFlow

[This tutorial](https://www.youtube.com/watch?v=c0k-YLQGKjY) was useful.

How to use:
1. Run the `lstm_train.ipynb` notebook  
    * This trains the LSTM model on hourly water level data from `2023-01-01` to `2023-07-31`. A window of the 10 previous water levels is used to predict the next water level. The first 4000 windows are used to train and the remaining are used for validation. The model is saved into a folder called `model1/`.
2. Run the `lstm_predict.ipynb` notebook
    * This loads the LSTM model from the `model1/` folder and tests how well it predicts hourly water level data between `2023-08-01` and `2023-08-31`, using the 10 previous water levels to recursively predict the next water level.  
