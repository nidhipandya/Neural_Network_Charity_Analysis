# Neural_Network_Charity_Analysis

### Overview of the analysis
A nonprofit called Alphabet Soup is looking to create a binary classifier that can analyze and predict whether applicants will be successful if they receive funding from the organization. The given dataset has more than 34,000 organizations who have received funding from Alphabet Soup is used to build the model. Using the dataset information and a deep learning model, we can help determine whether applicants will be successful with Alphabet Soup's funding.

### Results

#### Data Preprocessing

* What variable(s) are considered the target(s) for your model?
	* The column IS_SUCCESSFUL contains binary data, it referes to weither or not the charity donation was used effectively. This variable is considered as the target for the model.
* What variable(s) are considered to be the features for your model?
	* The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for the model.
* What variable(s) are neither targets nor features, and should be removed from the input data?
	* The variables EIN and NAME have been removed, because they are neither targets nor features. These two columns are simply identification for each row of data/each application (basically, identification for each and every data point); thus, they do not play a role in determining the outcome of a successful funding or not.

#### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
	* Initially, we used 80 and 30 neurons in two hidden layers respectively. also, we use ReLU activation fuction for the hidden layers and Sigmoid for output layer. As our output is a binary classification, Sigmoid is used on the output layer. 
* Were you able to achieve the target model performance
	* No, the level of accuracy achieved with this model was 72.51%, it's just below the target of 75%.
	![img1]
* What steps did you take to try and increase model performance?
	* The below steps we used to increase the model performace
		* Removed the noisy variables from features	
		* Added additional neurons to hidden layers (100,50)
		* Added additional hidden layers (3 hidden layers)
		* Changed the activation function of hidden layers (From ReLU to Sigmoid
		
### Summary

As this deep learning neural network model did not reach the target of 75% accuracy so we can considering that our achieved accuracy 72.51% is pretty average. we need binary outputs so we can try Random Forest Classifier to improve the model accuracy.
