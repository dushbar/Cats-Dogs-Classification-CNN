# Cats-Dogs-Classification-CNN
Classification using CNN

We create a CNN architecture to build a model which is trained on a labelled dataset consisting of images of dogs and cats.
We first use the tanh activation function throughout except for the output layer.
We observe overfitting so we use early stopping.

Then we use ReLU activation and we observe better results with less overfitting.

The dataset used is available here: https://www.kaggle.com/datasets/salader/dogs-vs-cats

Overfitting was observed. So data augmentation needs to be done to address this.
