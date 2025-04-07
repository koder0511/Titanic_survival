# Titanic_survival
Data is loaded from train.cv file.
Data preprocessing involves filling missing values, normalizing colums with messy values/high variation by taking log and getting rid of columns which do not offer much utility for training purpose by dropping them altogether.
Also, non-numeric values are transformed using fit_transform method of label encoder.
For exploratory data analysis, pivot tables are used to identify relation of certain columns with other ones (example: correlation of Survival with Sex, correlation of Survival with Passenger class and with Fare).
Data visualizaton is done by coming up with barplots, histograms, colourmaps to view correlation between variables and displot.
Model is trained on test_train split of 0.25 with cross_val score=5.
The model is trained on several models such as RandomForestClassifier, DecisionTreeClassifer, LGBMClassifier, XGBClassifier, Extra Trees Classifier and Logistic Regression.
Final accuracy of the predicted survival of passengers is 79.18 %.
