## digit-recognizer
project Description
MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

In this competition, your goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. We’ve curated a set of tutorial-style kernels which cover everything from regression to neural networks. We encourage you to experiment with different algorithms to learn first-hand what works well and how techniques compare.

## Implementation
1.Setting up the Project:
Installed Gradio, a Python library for creating user interfaces for machine learning models, and SHAP (SHapley Additive exPlanations) library, used for explaining model outputs.

2.Data Cleaning:
Checked and cleaned the data by handling missing values and removing duplications.

3.Data Preprocessing:
Scaled all pixel values to be between 0 and 1 (original range: 0 to 255).

4.Modeling and Training:

.Created a Keras model with input layer, 1 or 2 hidden layers, and an output layer with the number of classes in the target variable.
.Added regularization in the network.
.Used ReLU activation function between input and hidden layers, and between hidden and output layers.
.Applied softmax activation function after the output layer for class probabilities.
.Used a suitable loss function for multiclass classification problems.
.Determined predicted class based on the maximum probability.
.Utilized Adam optimizer, early stopping, and class weights to balance target variable classes.

5.Evaluation:
Printed a confusion matrix and classification report for model predictions on the validation set.

6.Deployment and Explainability:

.Utilized Gradio to enable uploading a grayscale 28 by 28 image and outputting the predicted class.
.Applied SHAP values on the uploaded image and displayed them in the Gradio app along with the predicted class.

By following these steps, the project is designed to handle data, train a multiclass classification model, evaluate its performance, and deploy it with explainability features using Gradio and SHAP.

