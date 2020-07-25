# Flood-Prediction-by-forecasting-using-ARIMA-model

## Disclaimer
So this method is rather an unconventional one. The problem given can be solved by using Logistic Regression and SVM models or alternatively by a Neural Network if the features are engineered properly. As we were asked to be as innovative as possible, I decided to go for Time Series Analysis using ARIMA model which is a quite complicated statistical model. As of now I don't understand the model completely and I'm studying it but i got help from the internet to understand and get a model up and running. Note that the code below does not generate the best model possible for the problem but with proper use of mathematical concepts and hyperparameter tuning this model could perform better than any other model possible.

## Model Summary
The main idea is to forecast the rainfall data for the next 10 years.
Then we calculate the standard deviation in the prediction data.
1. If the amount of rainfall entered by the user is more than (mean + std deviation) and (prediction + 0.7*std deviation) then we output 2 i.e: Flood is likely to occur
2. If the amount of rainfall entered by the user is more than (mean + std deviation) or (prediction + std deviation) then we output 1 i.e: There are chances of flood to occur.
3. Else we ouput 0 i.e: Flood is unlikely to occur.

*Note: I'm not using the Flood Dates sheet provided as I feel that the occurence of flood depends lot more on environmental and geographical factors than the history of flood occurences. This model cannot be generalized to all the areas. Some regions might get flooded on receiving 150 cm of rainfall while for some receiving 200-250 cm of rainfall is normal and does not cause any devastation.
