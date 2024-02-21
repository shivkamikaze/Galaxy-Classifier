# Galaxy-Classifier
Problem Statement and Dataset Description:
The objective of this project is to develop a robust classifier to categorize galaxies based on images obtained from the Sloan Digital Sky Survey (SDSS) dataset.
The SDSS dataset consists of images of galaxies with five different labels, representing distinct characteristics or classes of galaxies.

CNN Architecture and Keras Tuner Integration:
Constructed a Convolutional Neural Network (CNN) architecture using Keras, a high-level neural networks API.
Utilized Keras Tuner to perform hyperparameter optimization, automatically searching through a defined space of hyperparameters to identify the optimal configuration for the CNN model.
The CNN architecture consists of:
*convolutional layers: for feature extraction*
*pooling layers: to reduce spatial dimensions
*fully connected layers: for classification.

Preprocessing Techniques:
Addressed class imbalance issues present in the dataset by implementing preprocessing techniques.
Applied data augmentation to artificially increase the diversity of the training dataset by performing random transformations such as rotation, zooming, and flipping on the galaxy images.
Employed undersampling to mitigate the effects of class imbalance by randomly removing samples from the majority classes, ensuring a more balanced distribution of classes during training.

Model Training and Evaluation:
Split the dataset into training, validation, and testing sets to train and evaluate the performance of the CNN model.
Trained the model using the training set while validating its performance on the validation set to prevent overfitting.
Evaluated the trained model's performance on the testing set using metrics such as accuracy, precision, recall, and F1-score to assess its effectiveness in classifying galaxies across different classes.

Streamlit Deployment:
Developed a user-friendly interface using Streamlit.
Integrated the trained CNN model into the Streamlit application, allowing users to upload images of galaxies and receive real-time classification results.
