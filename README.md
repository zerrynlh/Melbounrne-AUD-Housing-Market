# Melbounrne Housing Market Prediction
Using machine learning to predict housing prices in Melbourne, Australia

This project uses compares decision tree and random forest algorithms to predict the price of homes in Melbourne, Australia. the data set was located on [Kaggle](https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot).

After cleaning the data, I performed correlation analysis to determine which numerical variables would be best for training the models. This determine that the variables with the strongest correlation to price were:

- Number of rooms
- Number of bathrooms
- Bedroom2 (room numbers from different source)
- Building area

The first model utilized was a decision tree which had a mean absolute error (MEA) of 256,665.

To improve the accuracy of predictions, a random forest algorithm was used which resulted in a 67,895 decrease in MEA.

After choosing the random forest algorithm, I performed tests by modifying the number of leaf nodes and decision trees to determined what the optimal leaf nodes and decision trees were. The final result was an MEA of 186,754.03 in home price prediction.
