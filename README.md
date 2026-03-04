-ROBUST-IMAGE-CLASSIFICATION-UNDER-ADVERSARIAL-AFFECTS


👕 Fashion MNIST Image Classification Using Transfer Learning

This project focuses on classifying fashion products using deep learning. By applying Transfer Learning with the VGG19 model, the system learns to recognize clothing categories from images in the Fashion-MNIST dataset.

The goal is to build an efficient image classification model that can accurately identify different fashion items such as shirts, shoes, bags, and dresses.

🚀 Project Objective

The main objective of this project is to develop an image classification pipeline using deep learning that:

Loads and preprocesses image datasets

Converts grayscale images to compatible formats

Uses transfer learning with VGG19

Trains a neural network for classification

Evaluates model performance using accuracy metrics

Identifies the most effective model configuration

🗂️ Dataset Description

The project uses the Fashion-MNIST dataset, which contains 70,000 grayscale images of fashion items.

Dataset split:

Training images: 60,000

Testing images: 10,000

Image size: 28 × 28 pixels

Classes in the Dataset

T-shirt / Top

Trouser

Pullover

Dress

Coat

Sandal

Shirt

Sneaker

Bag

Ankle Boot

🔧 Technologies & Libraries

The project was implemented using the following tools:

Python

TensorFlow / Keras

NumPy

Matplotlib

Transfer Learning (VGG19)

Deep Learning

🧹 Data Preprocessing

Several preprocessing steps were performed before training the model:

Normalized pixel values by dividing by 255

Converted grayscale images to 3-channel RGB images

Resized images to 32×32 to match VGG19 input requirements

Split the dataset into training and testing sets

🧠 Feature Extraction using Transfer Learning

The VGG19 model pretrained on ImageNet was used as the base model.

Key steps:

Loaded VGG19 without the top classification layers

Used the convolutional base as a feature extractor

Added custom dense layers for classification

🤖 Model Architecture

The final model consists of:

VGG19 Pretrained Base

Flatten Layer

Dense Layer

Softmax Output Layer

Architecture overview:

Input Image
     ↓
VGG19 Convolution Base
     ↓
Flatten Layer
     ↓
Dense Layer
     ↓
Softmax Output (10 Classes)
📈 Model Training

The model was trained with the following configuration:

Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Epochs: 1+ (can be increased for better performance)

Callback: Early Stopping

🏆 Results

The model successfully learned patterns in clothing images and classified them into correct categories.

Model	Description
VGG19 Transfer Learning	Deep learning model used for classification

Performance:

Achieved strong classification accuracy on the test dataset

Transfer learning significantly improved performance compared to training from scratch

📌 Conclusion

📊 This project demonstrates image classification using deep learning.

🧹 Image data was preprocessed and normalized for training.

🧠 Transfer learning using VGG19 helped extract powerful visual features.

🤖 A custom neural network was built on top of the pretrained model.

🏆 The model successfully classified fashion products into 10 categories.

🔍 Transfer learning reduced training time while maintaining strong accuracy.

🚀 This approach can be extended to real-world product recognition systems.

🔮 Future Improvements

Increase training epochs

Use data augmentation

Try advanced models like EfficientNet or ResNet50

Deploy the model with Streamlit or Flask

Build a real-time fashion product classifier
