# Premier League 2015-16 Analysis and Goal Prediction Model
![PL_Image_2](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/74b1148c-cce7-4c3b-9b11-372c0ea017f4)

## Project Overview

This repository offers an in-depth analysis of the historic Premier League 2015-16 season, with a focus on Leicester City's remarkable title-winning campaign. The analysis encompasses team performances, player contributions, and machine learning models for goal prediction. The dataset was obtained through StatsBomb's API and processed using Python libraries such as numpy and pandas.

## Data Description

### 1. Data
Encompasses the entire data journey, from initial extraction to exploratory data analysis (EDA) and visualizations. The collection of Jupyter notebook files within this directory meticulously documents each step of the process. Data extraction, data preprocessing, and the generation of insightful visualizations are systematically presented, offering transparency into the analytical journey.

### 2. Tables
Contains the tables extracted from the data collection process. These tables play a foundational role throughout the project. Organized and structured for optimal analysis, these tables provide the data backbone upon which the entire analysis is built. 

### 3. ML Model
Jupyter Notebooks focusing on the preprocessing of the collected data and its utilization in the development of machine learning models. The data undergoes careful processing to ensure its suitability for the models. This section highlights the creation, training, and evaluation of three distinct models, each contributing to the overarching analysis. Insights into the models' performance, accuracy, and predictive capabilities are detailed within this segment.

## Problem Aimed to Solve

The project addresses the goal of comprehensively analyzing the Premier League 2015-16 season, particularly Leicester City's iconic victory. Furthermore, it aims to demonstrate the application of machine learning models for predicting player goal contributions, which can be extended to broader contexts in modern football.

## Data Collection and Preprocessing

Data collection involved utilizing the `statsbombpy` library to access StatsBomb's API data. The collected data was meticulously organized and cleaned using Python's `numpy` and `pandas` libraries. Structured tables were created to represent various event groups within the 15/16 Premier League season.

#### Extracting the data using statsbombpy:
![Data_Extraction_1](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/9041e4c2-17ec-4e64-adb9-7ab7ad912d7e)

#### Collecting all the data for the 2015/16 Premier League season:
![Data_Extraction_2](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/07d8b090-c09c-4319-9042-3aa7e4a517a6)

#### Code to calculate the final table of the season:
![Table_Code](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/9b4f5081-e048-4ba4-93e7-36f08c5b7b02)

#### The final table of the 2015/16 Premier League season
![Table_Table](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/ede5ccda-1ee4-4ded-9d6f-8b57c8473018)

## Analysis

The analysis centers on the performances of the top 6 teams during the 2015-16 season. Metrics related to team performance, individual player statistics, and goal contributions were thoroughly examined. This exploration provided insights into the season's final standings and enabled comparisons of playing styles, strengths, and weaknesses.

#### Aggregation of the top 6 teams with key metrics
![DE_4](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/0f21a7fe-082d-4ba6-be65-3cb3843f9dad)

## Goal Prediction Models

In addition to the analysis, the project encompasses the development of machine learning models for goal prediction. 

#### Cleaning the data for usage in ML Models
![Model_1](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/aa9615d3-24cb-4c43-8c58-21abfcc80df8)

Two types of models were created to forecast player goal contributions.

### Linear Regression Model

A Linear Regression model, implemented using `scikit-learn`, effectively predicted the number of goals scored by players. With an accuracy of 0.88, this model demonstrated its efficacy in estimating goals based on diverse player events.

#### Fitting the linear regression model
![Model_2](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/4e425c54-42b0-4296-bb44-92a090a6ebe8)

#### Changing goals scored to a categorical column for classification models:
![Model_3](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/c03f89ce-214b-486e-b650-a8fd486e69b8)

### Classification Models

An alternative approach involved transforming the goal count into class intervals, leading to the creation of two classification models:

#### Logistic Regression

The Logistic Regression model achieved an accuracy of 0.80 and a weighted precision score of 0.79. It facilitated predictions of the goal range a player might achieve in the league.

#### Classification Report of the logistic regression model
![Model_4](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/77d86027-2f34-4d1f-81f3-c8ac6adf9f8a)

#### Confusion Matrix of the logistic regression model

![Model_4 5](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/36dff5ed-a5f6-4e2a-b48f-6f0ce50e18da)

#### Random Forest Classifier

Employing the Random Forest Classifier yielded an accuracy of 0.83 and a weighted precision score of 0.79. This ensemble learning technique was proficient in predicting goal ranges with considerable accuracy.

#### Classification Report of the Random Forest model
![Model_5](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/7cd9d191-cd3c-48b7-9d7c-3ddae36f98ba)

#### Confusion Matrix of the Random Forest model
![Model_5 5](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/5517b2ca-51d2-419d-843b-d695bd053280)

## Visualizations

#### Goals Scored vs Expected Goals amongst top scorers:
![Viz_1](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/a0fe172f-3afc-4bc6-bd4d-e226d6f33045)

#### Bad behaviour incidents per game amongst the top 6:
![Viz_2](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/ec6e226c-bea4-4bd2-b113-c86ca6f8ad88)

#### Top assists:
![Viz_3](https://github.com/harshahari8/Leicester_League_Analytics_15-16/assets/133602303/60b5bc73-25f4-4563-9784-c2a2eae0f49d)

## Learning, Limitations, and Challenges Faced

#### Learning New Skills
Undertaking this project brought forth valuable learning experiences. A significant aspect was acquiring proficiency in utilizing the StatsBomb API. Navigating the intricacies of API usage, understanding its endpoints, and effectively retrieving the required data presented a valuable learning curve.
#### Dealing with Highly Detailed and Enormous Data
One of the noteworthy challenges faced was handling the immense volume of detailed data acquired through the StatsBomb API. The nature of football data is highly granular, encompassing a multitude of events, players, and matches. Processing such detailed data demanded careful consideration of computational efficiency and memory management. Strategies for efficient data manipulation, aggregation, and visualization had to be devised to navigate the complexities posed by the size and richness of the dataset.

#### Data Quality and Completeness
Ensuring the quality and completeness of the data also posed a challenge. While the detailed data offered immense insights, it also necessitated careful data preprocessing and cleaning to address potential gaps, inconsistencies, or errors. Balancing the desire for granularity with the need for a coherent and accurate dataset demanded a rigorous approach to data quality assurance.

#### Integration of Machine Learning Models
The implementation of machine learning models introduced an additional layer of complexity. Preprocessing the data to make it suitable for modeling required meticulous attention. Tuning the models, handling feature engineering, and assessing their performance posed their own set of challenges. Balancing model complexity and interpretability, while striving for accurate predictions, required thoughtful experimentation and iteration.


## Conclusion

This project offers a comprehensive analysis of the historic Premier League 2015-16 season, highlighting Leicester City's monumental victory. The machine learning models developed here could be scaled to accommodate additional seasons' data and metrics, rendering them contextually relevant to contemporary football dynamics. As a valuable resource, this repository caters to football enthusiasts, data analysts, and machine learning aficionados keen on football analytics. The provided code, data, and visualizations invite further exploration for deeper insights.


## Libraries Used

- statsbombpy
- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn

## Note

Kindly note that the project's data originates from StatsBomb's free API, and the analyses and predictions rely on the available data. Additionally, the performance of the models may vary based on the dataset and features used.

## Acknowledgments

Our gratitude extends to StatsBomb for granting access to their data and to the open-source community for creating the libraries that facilitated this project. Special acknowledgment is reserved for the Python programming language for its versatility and user-friendly nature.

[![Additional Image](https://statsbomb.com/wp-content/uploads/2023/03/IconLockup_MediaPack-min.png)](https://statsbomb.com/wp-content/uploads/2023/03/IconLockup_MediaPack-min.png)
