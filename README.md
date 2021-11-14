# Neural_Network_Charity_Analysis


### Overview

The purpose of this analysis is using deep-learning neural networks using the TensorFlow platform in Python. It's to analyze and classify the success of charitable donations.

Here are the following methods used for this analysis:

  * Preprocessing the data for teh neural network model.
  * compile, train and evaluate the model
  * optimize the model.



### Resources

  * Python, Anaconda Navigator, Conda and Jupyter Notebook
  * Data Source: charity_data.csv



### Results 


* EIN and NAME are identification information and both have been removed from the input data.
* IS_SUCCESSFUL contains the binary data refering to weither if the charity donation was effective. The variable is then considered as the target for our deep learning neural network. 
* The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATION, ASK_AMT are the features for the model. Encoding of the categorical variables, spliting into training and testing datasets and standardization have been applied


### Compiling, Training, and Evaluating the Model


* The neural network model is made of two hidden layers with 80 & 30 neurons respectively. Input data has 43 features and 25,723 samples. The output layer is made of a unique neuron as it is the binary classification. In order to speed up the training process, we are using the ReLU for the hidden layers. As the output being the classification, we used Sigmoid on the output layer. 
* Model accuracy is showing under 75%. This number is not a satisfying performance to help predict the outcome of the charity donations. 
* To increase the performance model we had to apply bucketing to the feature ASK_AMT and organized the different values by intervals. We used the (tanh) activation function but none of the steps helped improved the performance. 


### Summary 

The deep learning neural network module did not pass the target reached of 75% accuracy. In consideration this target level is pretty average and can say that the model is not performaning to the standards. We should use a supervised machine learning model as the Random Forest Classifier to combine multitude of decision tree to generate a classified output and evaluate its overall performance against the deep learning model. 
