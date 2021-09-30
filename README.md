# TUMOR-CLASSIFICATION
This is a deep learning classification project to classify whether a tumor is malignant or benign on a breast cancer diagnosis dataset with keras in TensorFlow. 
EXPLORATORY DATA ANALYSIS

•	Used the Pandas info, head, describe and is null methods to do a quick exploration of the data.

•	Performed a count plot using seaborn visualization library to view the benign/malignant label in the data.

•	Checked the correlation between other features and benign/malignant feature in the data. 

**TRAIN TEST SPLIT, SCALING THE DATA AND CREATING OUR MODEL**

•	Selected our X and y variables and performed a train test split on them.

•	Scaled the X_train and X_test data to normalise them.

•	Created an artificial neural network using a sequential model and Dense layer.

•	I assigned the relu activation function to the first two neurons and used the sigmoid function for the final layer because we are solving a binary classification problem.

•	I used binary cross entropy for loss function and Adam optimizer.

•	Used the fit method to Train my training set and infuse new data (test data) into the model that it hasn’t evaluated before using validation data.

•	Plotted the train and validation loss with matplotlib which showed that the validation data was overfitting.

**OVERFITTING AND EVALUATION**

•	Used early stopping to stop training when there’s no need of improvement on the training data.

•	Also used drop put to ignore some neurons in our neural network to prevent overfitting.

•	Performed a prediction on Input test data, assigned a threshold of 0.5 so if the output is larger than 0.5, assign the input to class 1, otherwise assign it to class 0.

•	Used classification report and confusion matrix to evaluate our predictions performance with the initial test data.
