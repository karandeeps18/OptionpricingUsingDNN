# Option Pricing Using Deep Neural Networks

This project explores whether deep neural networks can learn to approximate the Black-Scholes option pricing partial differential equation (PDE). The focus is on pricing plain European call options using synthetic data generated from the Black-Scholes model.

## Codebase Overview

The codebase is structured as follows:

1. **Data Generation**: 
   - Synthetic option price data is generated using the Black-Scholes formula
   - Input features include: underlying price, strike price, time to maturity, risk-free rate, and volatility
   - Output is the theoretical option price

2. **Model Architecture**:
   - Deep Neural Network (DNN) with multiple hidden layers
   - Activation functions: ReLU or similar
   - Output layer with linear activation for regression

3. **Training**:
   - Model is trained on synthetic Black-Scholes data
   - Loss function: Mean Squared Error (MSE)
   - Optimizer: Adam or similar

4. **Evaluation**:
   - Model performance is evaluated on both training and test datasets
   - Metrics: MSE, MAE, and comparison to theoretical Black-Scholes prices

5. **Visualization**:
   - Plots comparing model predictions to theoretical prices
   - Error analysis and convergence plots

## Requirements
- Python 3.x
- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib

## Usage
1. Generate synthetic data using `data_generation.py`
2. Train the model using `train_model.py`
3. Evaluate and visualize results using `evaluate_model.py`

## Future Work
- Extend to other option types (puts, exotics)
- Incorporate market data
- Explore alternative neural network architectures