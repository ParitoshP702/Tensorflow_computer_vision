# Tensorflow_computer_vision
Created a binary classification deep learning model with Convolutional Neural Networks using tensorflow.
The dataset I used in the project is kaggle's Children vs Adults classification dataset(https://www.kaggle.com/datasets/die9origephit/children-vs-adults-images)
First of all I created a  convolutional neural network architecture using the Sequential API using 4 Conv2d layers and 2 MaxPooling layers(to reduce overfitting in our dataset)
Then we compiled the model, fitted the model in a history object and analysed the loss, validation loss, accuracy and validation accuracy by plotiing them using matplotlib. 
Then I used transfer learning feature extraction approach using the Functional API, using the inbuilt EfficientNetB0 model and  analysed the loss curves of our model.
I then further fine tuned the model by ungfreezing all the layers of our base model and compiled and fitted the modle with a 10 times lower learning rate and 5 extra epochs.
Created a function to calculate metrics like precision , recall, F1_score using scikit learn library.Also created a custom function to create and plot  the confusion matrix of our model.
Finally visualized the model using plot_model function in tensorflow.keras.utils class.
