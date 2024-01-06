Spiking Neural Network (SNN) Training on EMNIST Dataset
This repository contains a PyTorch implementation of a Spiking Neural Network trained on the EMNIST dataset using the Snntorch library. The SNN architecture includes convolutional layers with leaky spiking neurons and is trained through an Adam optimizer.

Key Features:
Neuron Initialization: Leaky spiking neuron parameters (beta and spike_grad) are initialized at the beginning, providing flexibility for experimentation with different values.
Optimizer Configuration: The Adam optimizer is employed with a learning rate of 3e-3 and specified betas. These hyperparameters may be adjusted for optimal performance.
Training Loop: The network is trained over multiple epochs, and training progress is visualized through plots of training loss versus iterations and test accuracy versus epochs.
Evaluation Metrics: Besides accuracy, consider exploring precision, recall, and F1-score as additional evaluation metrics, especially for imbalanced datasets.
Monitor training progress and explore techniques like learning rate scheduling or early stopping.
Feel free to adapt and extend this codebase to suit your specific goals and requirements for SNN model training.
