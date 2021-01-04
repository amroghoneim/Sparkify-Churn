# Sparkify-Churn

### Motivation:
Customer Churn, also known as Customer Attrition, is when the customer of a certain service stops using that service after a certain period of time. This proves troublesome for the service itself as it is of paramount importance to keep those customers for the sake of generating higher revenue.

Predicting customer churn is therefore an important task that many companies and service providers rely on to make sure their customers won't leave or stop using their service anytime soon. To meet this end, companies rely on a huge amount of data, usually known as Big Data, generated from the interactions of its users with its services, then analyze and model this data to be able to predict imminent churn for any given user.

In this Notebook, I will be using a dataset mimicking the interactions the users might have with popular music streaming services. The Sparkify dataset used here is a subset (128 MB) of the original (12 GB) dataset.

I will guide you through a machine learning solution created with Apache Spark's python API PySpark. I will explore, wrangle and model the dataset for the purpose of predicting users who will churn.

### python libraries needed:

Code was developed in Python 3.6.3 and the following libraries are needed:
- PySpark
- scikit-learn
- pandas
- numpy
- matplotlib

### Results

Using the logistic Regression Model, a Recall score of 77.8%, a Precision Score of 35% and an F1-score of 48% was achieved.
This means that the model was able to recall 77.8% of the users who did actually churn! However, with a precision score of 35%, the model
wrongly classified 65% of the users who did not churn and were happily using the service.

### Improvements

There is a huge room for improvement that can be done in many ways:
- Creating new features that take time into consideration
- Trying out different models such as Gradient Boost Tree Classifier
- Trying out different tuning parameters
- Some of the features generated here should be adjusted to take into account that some users' logs were recorded much later, towards the end of the dataset, than other users.
- Dealing with the outliers present in the dataset if any

### Licensing, Authors, Acknowledgements

Sparkify Data used was obtained from Udacity.

Otherwise, feel free to use the code!
