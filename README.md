# Deep Learning Challenge
The purpose of this project was to create a classifier able to predict successful investments into organizations using Deep Neural Net, TensorFlow, and Standard Scaler. For this, the data will be an extensive table with many columns giving information such as the list below, and the last one, is_successful, tells if the investment was successful of not.

* ein
* name
* application_type
* affiliation
* classification
* use_case
* organization
* status
* income_amt
* special_consideration
* ask_amt
* is_successful     

This data can be devided into 3 parts: the columns ignored, the features, and the target. The columns ignored are `ein` and `name`, `ein` is a primary key which makes it not viable when building a model, and `name` also doesn't help in feaguring out if an organization is worth investing into. The features are all the other columns except `is_successful` since each of them give some additional information about the organization and investment that can help building the model. And, the target is the last column `is_successful` that is used when training and testing the model to calculate the accuracy and error.

The model has 2 inner layers with 47 dimentions and 10 neurons each, and one output layer. The inner layers use the activation ReLu since this one gave the best accuracy for the models, and the output layer has the Sigmoid activation. The target model perfrmance for this project was an accuracy of 75%, however, even after making various modifications to the model, such as adding or subtracting layers or neurons, taking out columns, and changing the column bins.

After working on this model for some effort, it performed best at 73.99% and it is going to take guidance from someone more experience to better understand how to improve the performance of this model.
