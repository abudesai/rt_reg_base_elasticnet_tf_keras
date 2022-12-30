ElasticNet Regressor for Regression using TensorFlow/Keras

* elastic net
* tensorflow
* keras
* regularization
* activity regularizer
* neural network
* stochastic gradient descent
* python
* feature engine
* scikit optimize
* flask
* nginx
* gunicorn
* docker
* abalone
* auto prices
* computer activity
* heart disease
* white wine quality
* ailerons


This is an Elasticnet Regressor, a linear combination of L1 and L2 regularization, implemented using Tensorflow and Keras. 

The keras module provides with the required regularizer (l1_l2). A Stochastic gradient descent optimizer is used to reduce the overall loss and improve accuracy of the model. 

One Dense layer has been used in the Neural Network.

Preprocessing includes missing data imputation, standardization, one-hot encoding etc. For numerical variables, missing values are imputed with the mean and a binary column is added to represent 'missing' flag for missing values. For categorical variable missing values are handled using two ways: when missing values are frequent, impute them with 'missing' label and when missing values are rare, impute them with the most frequent. 

HPT includes choosing the optimal values for learning rate for the SGD optimizer and L1 and L2 regularization. 

The main programming language is Python. Other tools include Tensorflow and Keras for main algorithm, feature-engine and Scikit-Learn for preprocessing, Scikit-Learn for calculating model metrics, Scikit-Optimize for HPT, Flask + Nginx + gunicorn for web service. The web service provides two endpoints- /ping for health check and /infer for predictions in real time. 