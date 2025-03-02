# DL
The best performing model was determined based on its validation accuracy, achieving ~94% validation accuracy and ~88% test accuracy.
The model was trained for 5 epochs, ensuring effective learning without overfitting.
It consists of two fully connected layers with 128 neurons each, providing sufficient learning capacity.
Weight Decay (L2 Regularization): 0.0005 to prevent overfitting.
Learning Rate: 1e-3, allowing stable convergence.
Optimizer: Adam Accelerated Gradient Descent, effective for optimization.
Batch Size: 32, balancing computational efficiency and generalization.
Weight Initialization: Xavier, ensuring optimal weight distribution.
Activation Function: relu, promoting stable learning in deeper layers.
Training showed smooth convergence with balanced accuracy and loss.
The confusion matrix indicated high accuracy but some misclassification in similar characters.
Training showed smooth convergence with balanced accuracy and loss.
The confusion matrix indicated high accuracy but some misclassification in similar characters.
Validation Accuracy: Highest among all models.
Test Performance: Consistent with validation accuracy, minimal overfitting.
Training Behavior: Smooth convergence with well-balanced accuracy and loss.

Confusion Matrix Analysis:
High accuracy across most classes.
Some misclassification in visually similar characters.

Performance Metrics Validation Accuracy: 94.56% Test Accuracy: 88.28%

The dataset is divided into training and testing datasets. The 10% of large dataset is used for testing whereas the remaining data is used for training the model. A small portion of training dataset is also used for validation purpose.

Coding Style: The code follows a modular and flexible design. The create_model() function allows users to easily configure hidden layers, activation functions, optimizers, weight decay, and learning rate. This design ensures the model can be reused and modified easily for different experiments. The model supports multiple optimizers (SGD, Adam, RMSprop, etc.) and different weight initializations. It allows custom batch sizes and different numbers of hidden layers, making it adaptable for various experiments. The model is trained and tested using different possible combinations of hyperparameters.
