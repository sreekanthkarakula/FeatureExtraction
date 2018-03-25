# FeatureExtraction

This project is a rest service for doing feature extraction from IOT data.

This is backed by apache spark for loading data and extracting featues based on timestamp and the aggregation mode.

In a real world big data usecase there will be a request for new features to be extracted from the data.

Bascically the request for features extraction can be listened on a service through jms or kafka and once we have the request 
we take the features and the analytic has to know what aggregation techniques to apply for the collected features.

Usually a typical solution will be to save them as array of struct(to hive)/ feature vector for offline analysis. 
