# Melbourne Housing Market Prediction
Using machine learning to predict housing prices in Melbourne, Australia.

This project compares decision tree and random forest algorithms to predict the price of homes in Melbourne, Australia. The data set was located on [Kaggle](https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot).

After cleaning the data, I performed correlation analysis to determine which numerical variables had the strongest correlation to price. This determined that the variables with the strongest positive correlation to price were:

- Number of rooms
- Number of bathrooms
- Bedroom2 (room numbers scraped from a different source)

It should be noted that none of the numerical variables had a correlation coefficient greater than 0.5 so categorical variables were included using one-hot encoding.

Mutual information scores were obtained for each variable after label encoding which determined building area and postal code had the greatest MI scores.

Feature engineering was employed to add the ratio of land size to building area. Testing determined a moderate MI score of 0.14.

The first model utilized was a decision tree which had a mean absolute error (MAE) of 218,442..

To improve the accuracy of predictions, the random forest algorithm was used which resulted in a decrease in MAE.

After choosing the random forest algorithm, I performed tests by modifying the model to determine the optimal number of leaf nodes and decision trees. The final result was an MAE of 157,446 for price prediction. 

Cross-validation determined an MAE of 165,473 and scoring determined an R-squared value of 0.83.
