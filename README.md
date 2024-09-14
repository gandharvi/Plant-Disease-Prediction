# Leaf Disease Prediction

## Objective

The goal of this project is to develop a machine learning model capable of predicting leaf diseases from images. This model can assist farmers and agricultural professionals by providing accurate diagnoses based on images of plant leaves, thereby enabling timely and informed interventions.

## Dataset

The dataset used in this project is the [PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset) from Kaggle. This dataset contains images of healthy and diseased plant leaves, categorized by various plant species and their associated diseases.

- **Dataset Link:** [PlantVillage Dataset on Kaggle](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)
- **Dataset Description:** The dataset includes images of leaves categorized into different diseases and healthy conditions for various plant types.

## Model Used

The model employed in this project is a Convolutional Neural Network (CNN) based on the MobileNetV2 architecture, which is known for its efficiency and performance in image classification tasks. MobileNetV2 is used as a feature extractor with pre-trained ImageNet weights, and a custom classifier is added on top to adapt to our specific dataset.

### Model Architecture

- **Base Model:** MobileNetV2 (pre-trained on ImageNet)
- **Classifier:**
  - Flatten layer
  - Dense layer with 512 units and ReLU activation
  - Dropout layer with a rate of 0.5
  - Dense output layer with softmax activation to classify into one of 38 classes

### Model Training

- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy
- **Metrics:** Accuracy
- **Epochs:** 5

## Performance

The model achieved the following performance metrics:

- **Training Accuracy:** 86.3%
- **Validation Accuracy:** 91.3%

These results demonstrate the model's effectiveness in distinguishing between healthy and diseased leaves based on the provided dataset.


