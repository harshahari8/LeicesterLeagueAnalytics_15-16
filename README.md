# Premier League 2015-16 Analysis and Goal Prediction Model

This project provides an in-depth analysis of the Premier League 2015-16 season, Leicester City's historic title-winning campaign. The data was collected using StatsBomb's API and processed using Python libraries such as numpy and pandas. 

## Data Collection and Preprocessing

The `statsbombpy` library was utilized to access StatsBomb's free data via their API. The data was processed and organized using `numpy` and `pandas`. The cleaned and structured data was then used to create tables for different grouped events of the 15/16 Premier League season.

## Analysis

The analysis primarily focused on the top 6 teams' performance during the 2015-16 season. Various performance metrics, team statistics, and individual player goal contributions were examined to understand the finishing table of the season and compare playing styles, strengths, and weaknesses.

## Goal Prediction Models

In addition to the above, the data was also used to create machine learning models.
To predict the number of goals a player would score in the league, two types of models were created:

### Linear Regression Model

A linear regression model was implemented using `scikit-learn` to predict the number of goals for players. The model achieved an accuracy of 0.88, indicating its effectiveness in estimating goals based on various player events.

### Classification Models

For an alternative approach, the number of goals was transformed into class intervals, and two classification models were employed:

#### Logistic Regression

The logistic regression model achieved an accuracy of 0.80 and a weighted precision score of 0.79. This model allowed for the prediction of the range of goals a player might score in the league.

#### Random Forest Classifier

Using the Random Forest Classifier, an accuracy of 0.83 and a weighted precision score of 0.79 were obtained. This ensemble learning approach also proved useful in predicting goal ranges with satisfactory accuracy.

## Conclusion

This project provided an analysis of the Premier League 2015-16 season, which was special due to Leicester City's remarkable victory. 
This machine learning model approaches could be scaled to aggregate many more seasons' worth of data and metrics in order to be contextually relevant to the modern sport.
This repository serves as a valuable resource for football enthusiasts, data analysts, and machine learning enthusiasts interested in football analytics. The code, data, and visualizations presented here can be explored for further insights.

## Libraries Used

- statsbombpy
- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn

## Note

Please note that the data used in this project is sourced from StatsBomb's free API, and the analysis and predictions are based on the available data. Additionally, the models' performance may vary based on the dataset and features used.

## Acknowledgments

We extend gratitude to StatsBomb for providing access to their data and to the open-source community for developing the libraries that made this project possible. Special thanks to the Python programming language for its versatility and simplicity.

[![Additional Image](https://statsbomb.com/wp-content/uploads/2023/03/IconLockup_MediaPack-min.png)](https://statsbomb.com/wp-content/uploads/2023/03/IconLockup_MediaPack-min.png)


![Premier League](https://w7.pngwing.com/pngs/703/853/png-transparent-2016-17-premier-league-2015-16-premier-league-2018-19-premier-league-2013-14-premier-league-2017-18-premier-league-others.png)
