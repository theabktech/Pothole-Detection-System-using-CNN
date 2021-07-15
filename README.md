# Pothole-Detection-System-using-CNN
This is a pothole detection detection system created using Image Classification by Convolutional Neural Networks. 

### Dataset
The dataset consists of 3 folders : Train, Test and Validation(Val). All of the folders have images which are divided into two folders : Normal and Pothole. This has been done to label the images without creating a separate .csv file. The images used have been preprocessed into 64X64 image size to reduce the memory usage during the training of the model. The model has been designed for the same image size.
  1. Train - 1022 images divided into two classes
  2. Test -  136 images divided into two classes
  3. Val - 110 images divided into two classes
 
 Feel free to add more images to the dataset.
 
### Model
The model has been created using Keras library in Python. 
To injest the dataset into our model, we have used the ImageDataGenerator() function present in Keras. This function creates a "usable copy" of the image for the model to use for training and testing.
Multiple Convolutional 2D layers have been used in the model with 10 filters and ReLU activation function. The strides have varied (1,1) or (3,3) or (5,5). 
The output layer uses SoftMax Function. 
The loss function used is "Categorical Crossentropy", the optimizer used is "Adam" and the metrics used is "Accuracy".
Model has been run for 20 epochs and we got a validation accuracy of 91.82% which according to me is very good although I feel this might not be the case if we increase the dataset.

Feel free to add more images to the dataset to make this model more efficient.

Also, feel free to contact me via email (kulshreshthabhinav@gmail.com) if you have any suggestions for the model or you find a model better than this.
