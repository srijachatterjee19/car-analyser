# car-analyser 🚗

This car evaluation dataset composed of 1728 rows and 6 different attributes which are buying price, price of maintenance, number of doors, capacity in terms of persons to carry, the relative size of luggage boot and the estimated safety value of each car. The cars were classified using decision tree and random forests classifiers using Apache Spark’s ML library. The decision tree will classify the type of the car - 1) unacceptable, 2) acceptable, 3) good or 4) very good.

The classifier performances were then evaluated using the evaluate() method. The minimum instances per node when tweaked to a higher number seemed to produce less accuracy for the Random forests model.The decision tree model increased accuracy up to 92.38% after lowering the minimum instances per node to 2.Increasing the max depth to 30 and reducing the number of trees from 5 to 3, to 1 increased the accuracy to 89.94% but was indeed computationally expensive.It took longer to train and evaluate.
The accuracy and test errors for each model was then recorded.The Decision tree classifier performed better than the Random Forests classifier with the first getting an accuracy of 92.38%,test error 7.62% and 89.94% accuracy, 10.06% test error respectively.It was observed that 236 samples out of 241 of unacceptable car types were predicted better by the Random forests model than the decision tree which also signifies the samples for the car type unacceptable is higher than the other types.
