# Cats vs Dogs Classifier

A Convolutional Neural Network (CNN) built with TensorFlow/Keras to classify images as either cats or dogs. This project demonstrates the full workflow: data loading, preprocessing, model building, training, and evaluation in a Google Colab notebook.

The dataset used is available here: [Dataset](https://www.kaggle.com/datasets/chetankv/dogs-cats-images)

---

## Project Overview

- **Framework:** TensorFlow/Keras
- **Task:** Binary image classification (cats vs. dogs)
- **Input:** 256x256 RGB images
- **Output:** Probability of image being a cat or a dog

---

## Project Structure

.
├── CatsDogs_classifier_colab.ipynb # Main Colab notebook
├── README.md # Project documentation
└── dataset/
├── train/
│ ├── cats/
│ └── dogs/
└── test/
├── cats/
└── dogs/

## Model Architecture

- **3 Convolutional layers** (`tanh` or `ReLU` activation, 5x5 kernels, each followed by 2x2 MaxPooling)
- **2 Dense layers** (`tanh` or `ReLU` activation)
- **Output layer:** 1 neuron (sigmoid activation)
- **Optimizer:** Adam (learning rate 0.0001)
- **Loss:** Binary Crossentropy

  ## Training Results
 1. First `tanh` activation function was used without data augmentation which displayed overfitting.
 2. Early stopping was used but this did not address overfitting
 3. Then we used `ReLU` activation with data augmentation. This addressed the problem of overfitting
