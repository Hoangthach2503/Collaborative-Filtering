# Collaborative-Filtering
Product Recommendation on Santander Users Dataset taken from Kaggle (https://www.kaggle.com/c/santander-product-recommendation)

To predict which products their existing customers will use in the next month based on their past behavior and that of similar customers
It builds a logistic models using the existing products that a user has bought in the previous months, (and no other attributes) and creates one model for all the products in the 'upcoming month'.


The idea is to look at other customers with similar products, and recommend the customers the products that similar customers have purchased. This is done by running a LogisticRegression classifier to predict each product from the existing products a user has, essentially expressing each product as a linear combination of the other products. Then it is used to generate probabilities for the test set, and select the top 7 most likely products that people haven't already purchased in the training set.
