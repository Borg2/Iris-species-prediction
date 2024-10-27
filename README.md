# Iris-species-prediction

### **Introduction**

This repository contains a neural network model developed using PyTorch for classifying iris species based on their sepal and petal measurements. The model is trained on the classic Iris dataset, a widely used benchmark for machine learning tasks.The neural network is a simple two-layer fully connected feedforward model built with PyTorch.

### **Dataset**

The dataset used for training and evaluation is the Iris dataset, which consists of 150 samples from three species of iris (setosa, versicolor, and virginica). Each sample includes the following features:

* **sepal_length:** Length of the sepal in centimeters.
* **sepal_width:** Width of the sepal in centimeters.
* **petal_length:** Length of the petal in centimeters.
* **petal_width:** Width of the petal in centimeters.

### **Model Architecture**

Here's a sample description of the model architecture you can use for your README:

---

### Model Architecture

1. **Input Layer**: The model takes an input tensor of shape `(batch_size, 4)`, where 4 represents the number of input features.
   
2. **Hidden Layer**:
   - **Fully Connected Layer**: The first layer, `linear1`, maps the input of size 4 to an output of size 32.
   - **Activation Function**: A Sigmoid activation function is applied to introduce non-linearity, allowing the model to capture more complex relationships in the data.

3. **Output Layer**:
   - **Fully Connected Layer**: The second layer, `linear2`, maps the 32-dimensional input from the hidden layer to a 3-dimensional output, which represents the number of classes in the classification task.
   
4. **Loss Function**: CrossEntropyLoss is used as the loss function, suitable for multi-class classification.
   
5. **Optimizer**: Stochastic Gradient Descent (SGD) is used for optimization, with a learning rate of 0.02.

**Training Setup**: The model is trained in mini-batches of size 16, with data shuffled at each epoch to improve generalization.

### **Usage**

1. **Install dependencies:** Ensure you have the necessary libraries installed, including PyTorch, NumPy, and Matplotlib.
2. **Prepare data:** Load the Iris dataset and preprocess it as needed (e.g., normalize features, create training and testing sets).
3. **Train the model:** Run the training script to train the model on the prepared dataset.
4. **Evaluate performance:** Evaluate the model's performance using appropriate metrics such as accuracy, precision, recall, F1-score, and confusion matrix.

