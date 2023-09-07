# tides_lstm
Learning LSTMs in TensorFlow by predicting SF water levels

How to use:
1. Run the `lstm_train.ipynb` notebook  
    * This trains the LSTM model on hourly water level data from 2023-01-01 to 2023-09-01. A window of the 10 previous water levels is used to predict the next water level. The first 4500 windows are used to train and the remaining are used for validation. The model is saved into a folder called `model1/`.
2. Run the `lstm_predict.ipynb` notebook
    * This loads the LSTM model from the `model1/` folder and tests how well it predicts hourly water level data between 2023-08-20 and 2023-08-25, using the 10 previous water levels to predict the next water level.  
