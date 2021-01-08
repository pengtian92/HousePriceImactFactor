# Important Factor Analysis in House Pricing

House purchasing/selling is a very important project in everyone’s life. A deal would be made by considering many factors, such as location, quality, and space,etc. In this project, over 21613 transactions of house purchasing is investigated andreveal the importance factors of the house prices, in order. In this repo, the dataset I use is [House Sales in King County, USA](https://www.kaggle.com/harlfoxem/housesalesprediction), which contains 21613 sales transactions between May 2014 and May 2015 and each house has 19 attributes such as id, price, square feet in living room, square feet in lot, number of rooms, grades, etc. 

## Method
First, all of features in the dataset are normaized to zero mean and unit variacne. Second, a lasso-regularized linear regression is fitted with the normalized feature and the hourse prices. Mean squared error (MSE) is used as the metric and 5-fold cross-validation is employed to deterenming the regurlarization parameter. After obtaining the best peformaed regularization parameter, I train all the data in the single model with the optimal parameter. The top-10 important features are reported in the following figure.

![Important Factor](Importance-1.png)
