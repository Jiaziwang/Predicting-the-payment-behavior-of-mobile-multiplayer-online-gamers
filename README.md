# Predicting-the-payment-behavior-of-mobile-multiplayer-online-gamers
# Overview
This case study is a paid forecast of user behavior data for the SLG mobile game Brutal Age, which is a globally popular SLG mobile game. According to App Annie, "Age of Savagery" is the best-selling game in the top spot in 12 countries and in the top 10 in 82 countries. The game's advertising strategy and efficient operating activities (such as correct promotions and gift pack recommendations) contribute to a more personalized experience for players by accurately assessing the value of each player. Thus, we wish to be able to precisely determine the value of players from the moment they enter the game. In this competition, we will anticipate the total amount players will pay for each character within 45 days based on their behavior during the first seven days of their gaming experience.

* Data source: Chengdu Nibiru Technology Co., Ltd (English logo: tap4fun) provided to DC officials for the data competition
* Data size: millions
* Prediction type: regression
* Algorithms involved: Linear regression, logistic regression, random forest, GBDT

# Case Catalogue
**1.The gaming industry - a fast-growing new cultural and entertainment industry with new scenarios for data technology deployment**<br><br>
**2.From cash flow to revenue: a comprehensive analysis of the operations model for mobile games**<br><br>
**3.The sweet trap: how you move step by step towards consumption?**<br><br>
**4.Games and data: 6 typical scenarios in which data technology assists game operators**<br><br>
**5.Data exploration: in-depth exploration of game user behaviour data**<br>
- 1 Importing data and understanding basic data information<br>
    1.1 Understanding the characteristics of SLG game data<br>
    1.2 Missing/duplicate values<br>
- 2 Exploration of labels: important indicators of game operations and the current state of business<br>
- 3 Exploration of features<br>
    3.1 Length of time online: are users churning at a faster rate than normal?<br>
    3.2 Distribution and skewness: is the game newbie friendly? Is the game's difficulty set at a reasonable level?<br>
    3.3 Game balance: the impact of top-up consumption on the combat system<br>
    3.4 The left bias brings the long tail: who are the outlier players?<br>

**6.Model building: predicting user consumption behaviour**<br>
- 1 Importing libraries, integrating data<br>
- 2 Data pre-processing: correlation of registration time with consumption status<br>
- 3 Model selection, building a benchmark for the model<br>
- 4 Feature Engineering(1)：New features based on business model<br>
    4.1 New features based on new business indicators<br>
    4.2 New features based on business conclusions<br>
- 5 Feature Engineering(2)：Reaching the statistical assumptions required for modelling<br>
    5.1 Correlation analysis: screening features/feature importance<br>
    5.2 Adjustment of training/test set splitting<br>
    5.3 Outliers handling<br>
    5.4 Normalisation<br>
    5.5 Normalization process<br>
- 6 Model integration: dealing with extreme biases, anomalies and problems caused by the volume of data<br>
- 7 Model tuning/Optimisation<br> 

## 1.The gaming industry - a fast-growing new cultural and entertainment industry with new scenarios for data technology deployment

- Over the past 10 years, gaming has become one of the**most significant**forms of entertainment
> - The total value of global games in 2010 was about US$11 billion, now it is US$170 billion<br>**More than the total value of the global television and film industries combined**<br><br>
> - In 2009, the three gaming giants in the domestic market (Tencent, Shanda and NetEase) generated a total annual revenue of RMB 13.56 billion, while Tencent alone generated RMB 156.1 billion in gaming revenue in 2020, while NetEase generated RMB 54.61 billion<br>（This actually happens on top of the fact that a large number of games are available to play for free）<br><br>
> - Games become central to cultural life, with players focusing on deep systems/narratives/interactions and having the ability to appreciate and discriminate between games<br>**The main player base shifts from children to adults**<br><br>
> - The status of game participants/developers increases dramatically, eSports becomes an Olympic sport, anchors and game directors become superstars, politicians joke about PokemonGo in the presidential election, and there's a Fortnite dance at the World Cup ......

- The dramatic expansion of the industry, thanks to bold exploration and the course of history, is also linked to the lack of regulation<br><br>
- The rise of the mobile internet has fundamentally changed the status of the gaming industry
> - Mobile gaming has become the world's **most cash-grabbing** form of gaming<br>2000 - FC machines, arcade, handheld PSP, PC mainly<br>2010 - With the growth of the Internet, global PC game and online gaming expands dramatically<br>2021 - 76.37% of sales revenue from handheld games in China, 19.6% from PC games and 1.99% from online games<br>
> - The development of internet/digital mall/hardware technology has led to a dramatic expansion of gaming platforms/devices<br>The **threshold of access** to games has been dramatically reduced so that we don't have to go into an internet cafe/GameStop/sit at home to play games<br>This has led to a dramatic expansion of the **potential gaming population**, opening up the possibility of new profitable strategies and the establishment of a gaming culture<br>The development threshold for games has also been significantly lowered, with indie games emerging and large gaming companies needing to compete with smaller teams for creativity
<br><br>
> - The profit strategy has undergone a dramatic change, relying on the internet's conversion funnel which has become relatively mature.<br>In 2000, game copyright was sold offline (CDs / FC machine cards), requiring equipment / game software.<br>In 2005, game time was sold (prepaid cards) / participation rights (QQ game hall), and games required payment to participate.<br>By 2010, the model of free games with paid value-added services had taken shape, and many games survived at the cost of disrupting game balance<br>By 2020, the model of free games with paid value-added services had become mature, and efficient and easily acceptable payment models were everywhere<br><br>
> - A culture of gaming is gradually being established and the 'stigmatization of gaming' is improved<br>More respect for games staff

