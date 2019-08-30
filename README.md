# Tianchi_CarBrand_Prediction

[印象盐城 数创未来大数据竞赛 - 盐城汽车上牌量预测](https://tianchi.aliyun.com/competition/entrance/231641/information)

### Competition Background

Yancheng is the largest passenger vehicle manufacturing base in Jiangsu Province. The development of the automobile industry and the growth of urban automobile ownership pose challenges to urban construction and road planning. Predicting the overall automobile growth in Yancheng will play a guiding role in the government's road planning.


### Competiton Description 

In this competition, the player needs to use the history of the car to predict the number of cards every day for a certain 2 years. In the preliminary round, five car brands will be selected, and the number of cards each day will be given to predict the total number of car brands for the five car brands in the future. The semi-finals will select 10 car brands and still give the number of cards on the daily basis to predict the number of cards for the 10 car brands in the future.


# Competition results
No.45 in Preliminary Contest

No.81 in Final Contest

Total 2500 teams

# Solutions
1. Go back to real date: Verified the real date with the weekend and holiday pattern. The date period of preliminary contest is 2013-01-02 to 2017-11-28, while the date period of final contest is 2013-01-01 to 2017-11-28.

2. Labelled national holidays and festivals in both lunar and gregorian calendar to generate features. Taking brand, holiday_type, day_of_week, year, month, week_of_year (1-52) as features, where brand, holiday_type, day_of_week are used as categorical variables. 

3. Randomly select 0.1 as the validation set and submit the results of the LighGBM and CatBoost algorithm.
