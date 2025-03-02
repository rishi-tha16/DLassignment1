Key Observations
1.Adam optimizer consistently outperformed other optimizers (e.g., SGD, Momentum) in terms of speed and accuracy due to its adaptive learning rate.
2.ReLU activation was the most effective, as it avoided the vanishing gradient problem and facilitated faster convergence.
Sigmoid struggled, especially in deeper networks, due to vanishing gradients and slower convergence.
3.Adding more hidden layers and neurons improved performance to a point but caused overfitting beyond 4 layers and 64 neurons.
4.A learning rate of 1e-3 was ideal for most optimizers, providing the best convergence speed without instability.
5.Weight decay (L2 regularization) at 0.0005 helped prevent overfitting, but larger values led to poor performance.
6.Batch size of 32 worked well for balancing training time and model performance.
Best Performing Configuration:
Optimizer: Adam
Activation: ReLU
Hidden Layers: 3-4 layers
Neurons per Layer: 64
Batch Size: 32
Learning Rate: 1e-3
Recommendations for MNIST
1. Use Adam optimizer with a learning rate of 1e-3 for stable convergence.
2. Use 3 hidden layers with 128 neurons each for balanced performance.
3. Use ReLU activation for faster convergence compared to Sigmoid.
