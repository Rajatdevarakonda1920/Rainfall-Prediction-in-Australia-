# Rainfall-Prediction-in-Australia-
RainFall Prediction In Australia

Context
Predict next-day rain by training classification models on the target variable RainTomorrow.

Content
This dataset contains about 10 years of daily weather observations from many locations across Australia.

RainTomorrow is the target variable to predict. It means -- did it rain the next day, Yes or No? This column is Yes if the rain for that day was 1mm or more.

Implemneted using different classifers and comapred all the metrieces .
Model	Accuracy	Precision	True positive rate(recall)	True negative rate	False positive rate	train_score	test_score
0	Logistic Regression	0.851292	0.592	0.187	0.976	0.024	0.849511	0.851292
1	Logistic Regression_l2	0.852969	0.606	0.196	0.976	0.024	0.851066	0.852969
2	Logistic Regression_PCA	0.860167	0.665	0.23	0.978	0.022	0.858722	0.860167
3	DecisionTreeClassifier	0.797768	0.365	0.381	0.876	0.124	0.99997	0.797768
4	DecisionTreeClassifier_PRUN	0.846503	0.529	0.255	0.957	0.043	0.847396	0.846503
5	RandomForestClassifier	0.867242	0.743	0.243	0.984	0.016	0.999959	0.867242
6	RandomForestClassifier_Prun	0.865565	0.738	0.23	0.985	0.015	0.935293	0.865565
7	Naive Bayes	0.81628	0.407	0.359	0.902	0.098	0.816227	0.81628
8	KNeighborsClassifier	0.855043	0.571	0.330	0.953	0.047	0.890297	0.855043
9	SVC	0.85489	0.85489	0.869	0.095	0.997	0.003	0.853364	0.85489

Attribute Description:-
Date - The date of observation
Location - The common name of the location of the weather station
MinTemp - The minimum temperature in degrees celsius
MaxTemp - The maximum temperature in degrees celsius
Rainfall - The amount of rainfall recorded for the day in mm
Evaporation - The so-called Class A pan evaporation (mm) in the 24 hours to 9am
Sunshine - The number of hours of bright sunshine in the day.
WindGustDir - The direction of the strongest wind gust in the 24 hours to midnight
WindGustSpeed - The speed (km/h) of the strongest wind gust in the 24 hours to midnight
WindDir9am - Direction of the wind at 9am
WindDir3pm - Direction of the wind at 3pm
WindSpeed9am - Wind speed (km/hr) averaged over 10 minutes prior to 9am
WindSpeed3pm - Wind speed (km/hr) averaged over 10 minutes prior to 3pm
Humidity9am - Humidity (percent) at 9am
Humidity3pm - Humidity (percent) at 3pm
Pressure9am - Atmospheric pressure (hpa) reduced to mean sea level at 9am
Pressure3pm - Atmospheric pressure (hpa) reduced to mean sea level at 3pm
Cloud9am - Fraction of sky obscured by cloud at 9am. This is measured in "oktas", which are a unit of eigths. It records how many eigths of the sky are obscured by cloud. A 0 measure indicates completely clear sky whilst an 8 indicates that it is completely overcast.
Cloud3pm - Fraction of sky obscured by cloud (in "oktas": eighths) at 3pm. See Cload9am for a description of the values
Temp9am - Temperature (degrees C) at 9am
Temp3pm - Temperature (degrees C) at 3pm
RainToday - Boolean: 1 if precipitation (mm) in the 24 hours to 9am exceeds 1mm, otherwise 0
RainTomorrow - The amount of next day rain in mm. Used to create response variable RainTomorrow. A kind of measure of the "risk".
