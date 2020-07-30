# Anomaly-Detection-with-Isolation-Forest
Anomaly detection is the process of finding the outliers in the data, i.e. points that are significantly different from the majority of the other data points.
Large, real-world datasets may have very complicated patterns that are difficult to detect by just looking at the data.
That's why the study of anomaly detection is an extremely important application of Machine Learning.

Isolation forest is a machine learning algorithm for anomaly detection.
It's an unsupervised learning algorithm that identifies anomaly by isolating outliers in the data.
Isolation Forest is based on the Decision Tree algorithm. 
It isolates the outliers by randomly selecting a feature from the given set of features and then randomly selecting a split value between the max and min values of that feature.
This random partitioning of features will produce shorter paths in trees for the anomalous data points, thus distinguishing them from the rest of the data.
The Isolation Forest algorithm is based on the principle that anomalies are observations that are few and different, which should make them easier to identify.
Isolation Forest uses an ensemble of Isolation Trees for the given data points to isolate anomalies.

Isolation Forest recursively generates partitions on the dataset by randomly selecting a feature and then randomly selecting a split value for the feature. 
Presumably the anomalies need fewer random partitions to be isolated compared to "normal" points in the dataset, so the anomalies will be the points which have a smaller path length in the tree, path length being the number of edges traversed from the root node.
