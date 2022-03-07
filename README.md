# Machine Learning Trading Bot

![Decorative image.](Images/15-challenge-image.png)

## Description

In this challenge, I've assumed the role of a financial advisor at financial advisory firm. We compete with other major firms to manage and automatically trade assets in a highly dynamic environment. Here, I am improving the existing algorithmic trading system to maintain competitive advantage in the market. I do this by enhancing the existing trading signals with machine learning algorithms that adapt to new data.

### Libraries

Libraries used are pandas, numpy, hvplot, matplotlib and sklearn

# Summary Analysis

Please refer to the charts and classification reports below for different tunings and models explored building this machine learning trading bot.
![Baseline](Plots/Baseline.png)


## Tuning from Baseline SVM Model
The greatest impact to improving the baseline model is in tuning the training window. The short and long SMA window did not have much impact when tuned while maintaining the baseline training window at 3months. When tuning the training window, I made the adjustment from baseline of 3months to 12, 24, 36 and 48months. When tuned to 36months, the overall strategy performs the greatest when compared to the other training window models. 

Adjusting the SMA short and long windows alone, did not yield much impact when the baseline training window is maintained at 3months.

When tuning the parameters for both training and SMA windows, it was settled that the best performing SVM model is tuned to 36months with SMA windows set at 50 and 200.
![36-months](Plots/Tuned_36months.png)

## Exploring Additional Machine Learning Models
By optimizing the model further a variety of models were explored including, Logistic Regression, AdaBoost, Gradient Boosting Classifier, Decision Tree Classifier and Random Forest. Of the group classifiers, Random Forest is the best performing strategy as evidenced when compared to the other models.
![RandomForest](Plots/RandomForest.png)

---
## Baseline - SVM Model - 3-month Training Window + SMA Windows of 4 and 100 days



![Baseline](Plots/Baseline.png)

### Baseline - Classification Report
![Base](Classification_reports/Baseline.png)


## Adjusted Training Window - SMA Baseline Maintained at 4 and 100 days

![12-months](Plots/Tuned_12months.png)

![12-months](Classification_reports/Tuned_12months.png)

![24-months](Plots/Tuned_24months.png)

![24-months](Classification_reports/Tuned_24months.png)

![36-months](Plots/Tuned_36months.png)

![36-months](Classification_reports/Tuned_36months.png)

![48-months](Plots/Tuned_48months.png)

![48-months](Classification_reports/Tuned_24months.png)

## Adjusted Simple Moving Average (SMA) - Baseline Training Window Maintained at 3-months

![SMA50 and SMA100](Plots/SMA50-100.png)

![SMA50 and SMA100](Classification_reports/SMA50-100.png)

![SMA50 and SMA200](Plots/SMA50-200.png)

![SMA50 and SMA200](Classification_reports/SMA50-200.png)

## Adjust Training Window and SMAs

![12-months_SMA50-100](Plots/12months_SMA50-100.png)

![12-months_SMA50-100](Classification_reports/12months_SMA50-100.png)

![12-months_SMA50-200](Plots/12months_SMA50-200.png)

![12-months_SMA50-200](Classification_reports/12months_SMA50-200.png)

![24-months_SMA50-100](Plots/24months_SMA50-100.png)

![24-months_SMA50-100](Classification_reports/24months_SMA50-100.png)

![24-months_SMA50-200](Plots/24months_SMA50-200.png)

![24-months_SMA50-100](Classification_reports/24months_SMA50-200.png)

![36-months_SMA50-100](Plots/36months_SMA50-100.png)

![36-months_SMA50-100](Classification_reports/36months_SMA50-100.png)

![36-months_SMA50-200](Plots/36months_SMA50-200.png)

![36-months_SMA50-200](Classification_reports/36months_SMA50-200.png)

![48-months_SMA50-100](Plots/48months_SMA50-100.png)

![48-months_SMA50-100](Classification_reports/48months_SMA50-100.png)

![48-months_SMA50-200](Plots/48months_SMA50-200.png)

![48-months_SMA50-200](Classification_reports/48months_SMA50-200.png)

# Exploring Additional Machine Learning Models

![LogisticRegression](Plots/LogisticRegression.png)

![LogisticRegression](Classification_reports/LogisticRegression.png)

![AdaBoost](Plots/AdaBoost.png)

![AdaBoost](Classification_reports/AdaBoost.png)

![GradientBoostingClassifier](Plots/GradientBoostingClassifier.png)

![GradientBoostingClassifier](Classification_reports/GradientBoostingClassifier.png)

![DecisionTreeClassifier](Plots/DecisionTreeClassifier.png)

![DecisionTreeClassifier](Classification_reports/DecisionTreeClassifier.png)

![RandomForest](Plots/RandomForest.png)

![LogisticRegression](Classification_reports/RandomForest.png)