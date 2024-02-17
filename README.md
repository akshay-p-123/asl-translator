# asl-translator
![Usage of Program](https://github.com/akshay-p-123/asl-translator/assets/80610931/6d8c2b45-8cff-48ba-90d6-b5a82f1fcdeb)

A program created with NumPy, TensorFlow, Keras, and OpenCV to recognize American Sign Language from camera input.

This program utilizes a CNN (convolutional neural network) classification algorithm trained on a ~2,000 image subset of this [Kaggle Dataset](https://www.kaggle.com/datasets/grassknoted/asl-alphabet). TensorFlow and Keras are used to create the ML model, NumPy is used for data processing, and OpenCV is used to read image and camera data. While I could have used transfer learning to increase the algorithm's accuracy, my main intention in this project was to learn how to train and optimize a CNN in the context of image classification. I used data regularization, hyperparameter tuning (epochs, batches, optimization function), and dropout layers to decrease model overfitting and increase prediction accuracy. Python 3.7 is used as it is the latest version of Python compatible with TensorFlow on Windows.

Due to current hardware limitations, I struggled to optimize and train my model comprehensively with sparse data, which is why I limited the number of input features. To overcome this problem, I plan to implement a custom GridSearch algorithm to batch sparse data during hyperparameter tuning so not all of it is in memory at the same time. In addition, the model would not train when I employed data augmentation techniques outside of the RandomFlip layer. This is another problem I plan to fix. Furthermore, I will make this program into a script.

Instructions for running the program are in the Jupyter Notebook. Only run the cells that say "Run this."
