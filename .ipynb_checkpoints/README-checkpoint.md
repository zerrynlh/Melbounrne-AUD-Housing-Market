# Melbourne Housing Market Prediction
Using machine learning to predict housing prices in Melbourne, Australia.

This project compares decision tree and random forest algorithms to predict the price of homes in Melbourne, Australia. The data set was located on [Kaggle](https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot).

After cleaning the data, I performed correlation analysis to determine which numerical variables had the strongest correlation to price. This determined that the variables with the strongest positive correlation to price were:

- Number of rooms
- Number of bathrooms
- Bedroom2 (room numbers from different source)

It should be noted that none of the numerical variables had a correlation coefficient greater than 0.5 so categorical variables were included using one-hot encoding.

The first model utilized was a decision tree which had a mean absolute error (MAE) of 228,166.

To improve the accuracy of predictions, the random forest algorithm was used which resulted in a decrease in MAE to 205,139.

After choosing the random forest algorithm, I performed tests by modifying the number of leaf nodes and decision trees to determined what the optimal leaf nodes and decision trees were. The final result was an MAE of 156,356 in home price prediction. Cross-valiation determined a MAE of 167,959.
