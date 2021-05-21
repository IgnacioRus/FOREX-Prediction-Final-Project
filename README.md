<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# FOREX Prediction
*[Ignacio Rus Prados]*

*[DAFT MAR21, Remote, 20/05/2021]*

## Content
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Analysis](#analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Links](#links)

## Project Description
I have set up a Machine Learning model to analyze FOREX historical data and try to predict the change in price. In particular, I will examine the EUR/USD currency pair.

## Dataset
The data was collected from https://www.investing.com/currencies/eur-usd-historical-data. A daily time frame was chosen and data from 01/01/2002 to 01/01/2021 was downloaded. This included opening and closing prices for each day, as well as the maximum and minimum prices reached during the day.

## Analysis
Before deploying our Machine Learning model, a variety of econometrics indicators were calculated to encapsulate all the essential information about the price evolution. Relevant indicators such as RSI, MACD, ADX and both regular and exponential moving averages with different periods were added. The correlation between these features and the change in price was minimal, which shows the stochastical nature of the problem.

## Model Training and Evaluation
The Machine Learning algorithm used was GradientBoostingClassifier(), which was complemented with an scaler (StandardScaler, although RobustScaler was also tested and showed generally worse results) to prepare the data for model training. The data was splitted into a training set (60%), validation set (20%) and test set (20%).

Several models were trained and tested, starting with simple models and consecutively adding improvements and fine-tuning the model parameters.

Regarding the evaluation, the accuracy was calculated both in the train and test set. The accuracy score for the test set was never over 60%, so the Cohen's Kappa score was also calculated in order to test how likely it was that our results were signicant or just a matter of chance.

## Conclusion
Despite the amount of tries and different techniques used, it was concluded that, with the time limitations of this project and my current understanding of FOREX market, it was not possible to find a model that can consistently make accurate predictions.

## Links

[Repository](https://github.com/IgnacioRus/FOREX-Prediction-Final-Project)  
[Slides](https://www.canva.com/design/DAEfA134LNY/EefpYftt9b9kROeWNksa7Q/edit#)  
[Trello](https://trello.com/b/xZ84Ljv6/forex-prediction-final-project)  
