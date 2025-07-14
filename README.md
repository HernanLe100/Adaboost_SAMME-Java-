# Adaboost_SAMME_Java
An Adaboost SAMME model built entirely from scratch without any fancy libraries other than Java's built-in packages


WeakLearner.java
- the decision stump for the model
- divides the input data into two sides and tries to maximize the weighted sums of the assigned labels

BoostingAlgorithm.java
- creates multiple decision stumps to make a prediction
- weight of each data point is modified after each iteration so the next stump can try to correctly classify it
- each weak learner is also assigned an amount of say based on its individual training error which will correspond to its weight in the final accumulated prediction
