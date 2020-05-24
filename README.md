# Prediction-of-RUL-of-an-aircraft
I implemented a model with a combination of ​Random Forest ​for predicting ​HI(​Health Index) and an ​LSTM​(Long Short Term Memory) neural network for predicting the ​RUL​(Remaining Useful Life). ​HI ​indicates the probability of a given state to be healthy which is achieved by taking probability of predicted outcomes of all decision trees of a random forest.This obtained HI is used as one of the features along with 9 sensors,Time cycle and Operational setting for training LSTM network. This LSTM network takes 50 consecutive time steps, 12 features as input and predicts the last time step’s RUL. For prediction,the last 50 cycles of each engine of the test set are considered as input  and for engines having less than 50 time cycles an RUL of 125 is assumed. The best score obtained by the above approach is ​1131​.
