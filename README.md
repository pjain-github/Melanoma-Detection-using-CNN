# Melanoma Detection using Convolutional Neural Networks (CNN)

## Overview

This project aims to build a CNN-based model that can accurately detect melanoma, a deadly type of skin cancer. Early detection of melanoma is crucial for successful treatment, and this solution has the potential to reduce manual effort in diagnosis.

## Dataset

The project utilizes a dataset of about 2357 images of skin cancer types, divided into 9 sub-directories for each type. The dataset is split into training and testing sets.

## Steps Involved

1. **Data Preparation:**
    - Import necessary libraries, including TensorFlow, Keras, and Matplotlib.
    - Mount Google Drive to access the dataset.
    - Define paths for training and testing data.
    - Load images using `image_dataset_from_directory`, resizing them to 180x180 pixels.
    - Visualize the data to understand the different skin cancer types.

2. **Model Building:**
    - Create a CNN model with layers for convolution, max pooling, batch normalization, dropout, and dense connections.
    - Use `Rescaling` to normalize pixel values between 0 and 1.
    - Compile the model with an appropriate optimizer and loss function.

3. **Model Training:**
    - Train the model using the training dataset.
    - Monitor training and validation accuracy and loss.
    - Visualize training results to identify potential overfitting or underfitting.

4. **Data Augmentation:**
    - If overfitting is observed, apply data augmentation techniques using the `Augmentor` library.
    - Visualize augmented images to ensure they are diverse.
    - Retrain the model with the augmented dataset.

5. **Class Imbalance:**
    - Analyze the distribution of classes in the training dataset.
    - Rectify class imbalance using Augmentor to add more samples to under-represented classes.

6. **Model Evaluation:**
    - Evaluate the final model on the test dataset.
    - Report accuracy, loss, and other relevant metrics.

7. **Prediction:**
    - Load a test image and make a prediction using the trained model.
    - Display the predicted class and compare it to the actual class.


## Final Performance

- **Accuracy:** 
- **Validation Accuracy:**
- **Loss:**
- **Validation Loss:**

## Findings and Conclusion

- The initial model showed signs of overfitting.
- Data augmentation and class rebalancing techniques helped to mitigate overfitting and improve model performance.
- The final model achieved an accuracy of [insert accuracy] on the test dataset.
- The project demonstrates the potential of CNNs for skin cancer detection and highlights the importance of addressing overfitting and class imbalance.


## Additional Notes
* The model can be further improved by experimenting with different architectures, hyperparameters, and augmentation strategies.
* The dataset used in this project is relatively small, and using a larger and more diverse dataset could further enhance performance.
* This model is intended for educational and research purposes only and should not be used for clinical diagnosis without further validation and approval.
