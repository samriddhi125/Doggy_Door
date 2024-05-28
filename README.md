# Automated Doggy Door

Welcome to the Automated Doggy Door project! This project utilizes a pre-trained VGG16 model to create an intelligent doggy door that distinguishes between dogs, cats, and other animals, allowing only dogs to pass through and not letting cats go out while keeping other animals outside.

Ensure you have the following Python packages installed:
- TensorFlow
- NumPy
- Matplotlib

The ImageNet weights for the VGG16 model will be downloaded automatically when you load the model using TensorFlow.

## Usage

### Loading the Model

First, we load the VGG16 model pre-trained on the ImageNet dataset. This model will be used to classify images and make decisions based on the predictions.

### Loading an Image

Next, we load an image and display it. This step is crucial for visual verification and ensuring that the correct image is being processed.

### Preprocessing the Image

Images need to be preprocessed to fit the input requirements of the VGG16 model. This involves resizing the image, converting it to a numerical array, and applying the same preprocessing steps used during the model's training.

### Making a Prediction

We use the pre-trained model to make predictions on the processed image. The predictions are decoded to readable labels, showing the top three predictions with their probabilities.

### Doggy Door Function

Finally, we implement the logic for the doggy door. Based on the model's predictions, the function determines if the animal in the image is a dog, a cat, or another animal. Dogs are allowed to pass through, while cats and other animals are kept outside.
