# Predicting-the-payment-behavior-of-mobile-multiplayer-online-gamers
# Overview
This case study is a paid forecast of user behavior data for the SLG mobile game Brutal Age, which is a globally popular SLG mobile game. According to App Annie, "Age of Savagery" is the best-selling game in the top spot in 12 countries and in the top 10 in 82 countries. The game's advertising strategy and efficient operating activities (such as correct promotions and gift pack recommendations) contribute to a more personalized experience for players by accurately assessing the value of each player. Thus, we wish to be able to precisely determine the value of players from the moment they enter the game. In this competition, we will anticipate the total amount players will pay for each character within 45 days based on their behavior during the first seven days of their gaming experience.

* Data source: Chengdu Nibiru Technology Co., Ltd (English logo: tap4fun) provided to DC officials for the data competition
* Data size: millions
* Prediction type: regression
* Algorithms involved: Linear regression, logistic regression, random forest, GBDT

# Case Catalogue
1.The gaming industry - a fast-growing new cultural and entertainment industry with new scenarios for data technology deployment

2.From cash flow to revenue: a comprehensive analysis of the operations model for mobile games

3.The sweet trap: how you move step by step towards consumption?

4.Games and data: 6 typical scenarios in which data technology assists game operators

5.Data exploration: in-depth exploration of game user behaviour data

1 Importing data and understanding basic data information
1.1 Understanding the characteristics of SLG game data
1.1 Missing/duplicate values
Exploration of labels: important indicators of game operations and the current state of business
Exploration of features
3.1 Length of time online: are users churning at a faster rate than normal?
3.2 Distribution and skewness: is the game newbie friendly? Is the game's difficulty set at a reasonable level?
3.3 Game balance: the impact of top-up consumption on the combat system
3.4 The left bias brings the long tail: who are the outlier players?
6.Model building: predicting user consumption behaviour

Importing libraries, integrating data
Data pre-processing: correlation of registration time with consumption status
Model selection, building a benchmark for the model
Feature Engineering(1)：New features based on business model
4.1 New features based on new business indicators
4.2 New features based on business conclusions
Feature Engineering(2)：Reaching the statistical assumptions required for modelling
5.1 Correlation analysis: screening features/feature importance
5.2 Adjustment of training/test set splitting
5.3 Outliers handling
5.4 Normalisation
5.5 Normalization process
Model integration: dealing with extreme biases, anomalies and problems caused by the volume of data
Model tuning/Optimisation
