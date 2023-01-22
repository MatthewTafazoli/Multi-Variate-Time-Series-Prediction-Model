# Multi-Variate-Time-Series-Prediction-Model
Model to predict future predator/prey population numbers (Lotka-Volterra equations), based on past population numbers. 

The model uses a Long Short-Term Memory (LSTM) RNN architecture, with a lookback period of 20. The dataset contains 2000 time step values for x and y (predator and prey population numbers), however contains many rows missing either x or y values. This issue was patched up using several methods, the most effective of which being data imputation. 

The model achieves test loss of ~.07 and train loss of ~.12 after a relatively short 100 epochs of training. When comparing the predicted values to the dataset's values, the numbers line up quite well (please reference the below images, as well as the google colab that the code is hosted on for more information).

![Screenshot_9](https://user-images.githubusercontent.com/77253145/213919193-d6237e44-4954-4494-897d-f8d713773792.png)
![Screenshot_10](https://user-images.githubusercontent.com/77253145/213919194-39cf996c-c4c5-41d3-b441-5b707db65871.png)
![Screenshot_11](https://user-images.githubusercontent.com/77253145/213919195-afbb334a-b1d4-4400-9cba-497304989c5a.png)
