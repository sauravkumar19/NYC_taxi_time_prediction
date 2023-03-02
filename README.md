# NYC_taxi_time_prediction
Problem Statement

First of all before going through any code or analysis we must know what is the reason for doing this
analysis.
Data provided to us have many attributes which refer to a particular trip, our task is to remove noise
from that data, and then find relation among the different attributes, to visualize the behavior of
attribute or relation of two or more attributes using eda. To gain understanding from the data, we will
use Python to undertake exploratory data analysis.

Our task involves to build a model that predicts the total ride duration of taxi trips in New York City.
our primary dataset is one released by the NYC Taxi and Limousine Commission, which includes
pickup time, geo-coordinates, number of passengers, and several other variables.



Conclusion

● Total_distance, pickup_shift, is_weekend feature were found to be most
relevant for predicting the trip duration for NYC taxi.

● From pickup_shift it is clearly visible that, at lunch time taxi takes long time to
cover short distance, whereas at midnight taxi takes short time to cover long
distance. This implies people face lots off traffic during lunch time.

● In weekends people usually book a taxi for a longer trip.

● Most of the taxis do not have store and forward flag but for long duration a
taxi with store and forward flag is preferred.

● Our dependent column taxi trip mostly have data of shorter trips.

● Linear regression model does not perform good in this dataset as very few
dependent variable is strongly correlated to independent variable. The XGB
and GBM provide substantial improvement in predicting the trip duration. The
root mean square error is less than 300 seconds and r2 and adjusted r2 score
is 0.79.

● So we used XGboost and Gradient boost model for prediction,. This model
can also improve by finer tuning of hyperparameters.
