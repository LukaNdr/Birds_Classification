# Bird Classification using Convolutional Neural Networks

## Overview

This repository contains code for training a Convolutional Neural Network (CNN) to classify bird images into different species. The dataset used for this project consists of bird images, and the model is designed to predict the species of a bird given its image.

## Project Structure

- **data/:** This directory contains the bird images organized into subfolders, each representing a different bird species. These images are used for training and testing the model.

- **drive/:** The directory where the Google Drive files are stored.

- **requirements.txt:** A file containing the necessary Python packages and their versions. You can install these dependencies using `pip install -r requirements.txt`.

- **bird_classification.ipynb:** The main Jupyter Notebook file containing the code for loading the dataset, building and training the CNN model, and visualizing the results.

## Usage

1. **Setup Environment:**
   - Install the required dependencies using `pip install -r requirements.txt`.
   - Ensure that the bird images are organized in the `data/` directory with subfolders for each bird species.

2. **Data Preprocessing:**
   - The script loads and preprocesses the bird images. Images are resized to (224, 224) pixels and normalized to the range [0, 1].
   - The dataset is split into training and testing sets.

3. **Model Architecture:**
   - The CNN model is defined using the Keras Sequential API.
   - It consists of convolutional layers with max-pooling, followed by fully connected layers.
   - The model uses the Adam optimizer and categorical cross-entropy loss for training.

4. **Data Augmentation:**
   - Image data augmentation is applied using the `ImageDataGenerator` to improve model generalization.
   - Augmentation includes rotation, width and height shift, shear, zoom, and horizontal flip.

5. **Training:**
   - The model is trained using the training set with a learning rate schedule and early stopping to prevent overfitting.
   - Training progress is visualized, including accuracy and loss metrics.

6. **Testing:**
   - The trained model is evaluated on the testing set, and test accuracy is reported.

7. **Visualization:**
   - Predictions on sample test images are visualized, showing the actual and predicted bird species.
   - Test Loss: [0.7891]
   - Test Accuracy: [0.7660]
  
   - ![image](https://github.com/LukaNdr/Birds_Classification/assets/147658141/f7aa81f4-43db-4ff4-94de-b02333d10388)



## Results

- The trained model achieves a certain accuracy on the test set, demonstrating its ability to classify bird species.

- Visualization of predictions on sample images provides insights into the model's performance.

## Acknowledgments

- The dataset used for this project is sourced from [https://drive.google.com/drive/folders/1rvBpZG6_7YG1xPQc_roCgF3DFvlLRja4?usp=drive_link].

## Author

[Luka Nadiradze]

## Vizualizing results

![image](https://github.com/LukaNdr/Birds_Classification/assets/147658141/0a7e15ba-89f1-4670-b453-37414e095a78)

![image](https://github.com/LukaNdr/Birds_Classification/assets/147658141/78e3d8ea-3cbf-4ad1-b882-1f8be57a095b)

