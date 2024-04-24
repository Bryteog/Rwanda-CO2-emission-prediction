### Rwanda-CO2-emissions-prediction

<hr>
Completed as part of the kaggle [competition](https://www.kaggle.com/competitions/playground-series-s3e20), where participants are required to predict the CO2 emissions of a locale given data of surrounding areas.
The [data](https://www.kaggle.com/competitions/playground-series-s3e20/data) is obtained from the site page for the competition.

<hr>
The predicted value is discrete as this is a regression task. The XGBoost algorithm was used for modelling. The dataset is large having 143 labels (excluding the target), and many labels had numerous missing values.
Imputation with the mean or median was tried but gave a very poor performing model with MSE > 2400!. Observing submissions by other participants I noticed the use of feature engineering and the significant improvement it had on model
performace hence applied it.
The MSE after engineering new features from the latitude and longitude was ~23.5! which is far better than even the other submissions inspiration was taken from. <bold>b</bold>
