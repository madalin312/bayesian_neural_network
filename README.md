# bayesian_neural_network

# Bayesian Neural Networks

## Overview
This project involves the implementation and training of Bayesian Neural Networks (BNNs) using Markov Chain Monte Carlo (MCMC) methods for categorical and binary classification tasks. The project was completed as part of the Probabilistic Programming course at the Polytechnic University of Bucharest.

## Project Structure

- **Task**: The primary task is to build a Bayesian Neural Network and train it using MCMC to perform both multi-label (categorical) and binary classifications.
  
- **Implementation**: 
  - **Multi-label Classification**: The Iris dataset is used for this task, which involves classifying data into three categories based on four input features.
  - **Binary Classification**: Randomly generated points are used to differentiate between "real" and "fake" points. The input features consist of two values (x and y coordinates), and the output is the probability of a point being "real."

- **Model Architecture**:
  - For multi-label classification, the input layer has 4 neurons corresponding to the 4 features in the Iris dataset, and the output layer has 3 neurons for the three possible classes.
  - For binary classification, the input layer has 2 neurons (x and y coordinates), and the output layer is a single neuron representing the probability of a point being "real."

- **Libraries Used**: The Flux library in Julia was used to create and manage the neural networks. Flux also simplifies the process of recalculating weights and biases, facilitating the construction of generative functions and setting up model constraints.

## Results
- **Multi-class Classification**: The Bayesian Neural Network achieved nearly perfect accuracy in under 10 epochs.
  - Accuracy for BNN, multi-class classification: **Near-perfect accuracy**
  
- **Binary Classification**: The predicted probability for the "real" points reached approximately 0.86 after 10 epochs.
  - Accuracy for BNN, binary classification: **0.86 probability**

- **Comparison with Traditional Neural Networks**:
  - The Bayesian Neural Networks demonstrated superior performance metrics compared to traditional neural networks. Additionally, the BNNs were more time-efficient, requiring less time for training while achieving better results.

## How to Run
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2. **Install Dependencies**:
    - Ensure you have Julia installed.
    - Add the necessary packages by running:
    ```julia
    using Pkg
    Pkg.add("Flux")
    Pkg.add("Distributions")
    Pkg.add("Turing")
    ```

3. **Run the Project**:
    - You can run the project scripts in a Julia environment or using a Jupyter notebook with Julia kernel.

4. **Evaluate the Results**:
    - The scripts will output accuracy metrics for both the multi-class and binary classification tasks. Compare the performance of the Bayesian Neural Network with that of a traditional neural network.

## Bibliography
- [Deep Learning with Julia](https://medium.com/coffee-in-a-klein-bottle/deep-learning-with-julia-e7f15ad5080b)
- [How to Build an Artificial Neural Network from Scratch in Julia](https://towardsdatascience.com/how-to-build-an-artificial-neural-network-from-scratch-in-julia-c839219b3ef8)
- [Build Your First Neural Network with Flux.jl in Julia](https://towardsdatascience.com/build-your-first-neural-network-with-flux-jl-in-julia-10ebdfcf2fa3)
- [Julia Tutorials on GitHub](https://github.com/julia4ta/tutorials/tree/master/Series%2005/Tutorial%2005x08)

## Author
- **Radu Madalin-Cristian**, Group 407, Polytechnic University of Bucharest
