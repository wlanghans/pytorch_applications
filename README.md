# PyTorch Applications

PyTorch-based applications motivated by real-world problems in dynamical systems simulation and optimization.

## Project Structure

```
pytorch_applications/
├── README.md
├── requirements.txt
└── lorenz/
    ├── lorenz_ekf.ipynb
    └── optimize_lorenz.ipynb
```

## Folder Overview

### `lorenz/`
This folder contains Jupyter notebooks focused on the Lorenz dynamical system, a classic non-linear system that exhibits chaotic behavior. The notebooks demonstrate different applications of PyTorch for scientific computing:

#### **[lorenz_ekf.ipynb](lorenz/lorenz_ekf.ipynb)**
State estimation for the Lorenz system using an Extended Kalman Filter (EKF).

**PyTorch Usage:**
- Leverages PyTorch's automatic differentiation (autograd) to compute Jacobian matrices automatically
- Implements the Lorenz equations as a differentiable function using PyTorch tensors
- Enables efficient computation of derivatives required by the EKF algorithm without manual implementation

**Key Topics:**
- Non-linear dynamical system simulation
- Extended Kalman Filter for state estimation
- Automatic differentiation for Jacobian computation
- Handling noisy observations in chaotic systems

#### **[optimize_lorenz.ipynb](lorenz/optimize_lorenz.ipynb)**
Parameter optimization for the Lorenz system using backpropagation in time for gradient-based methods.

**PyTorch Usage:**
- Uses PyTorch's autograd to compute gradients of the loss function with respect to system parameters
- Implements multiple optimization strategies including single-scenario and online optimization
- Demonstrates iterative parameter tuning through gradient descent

**Key Topics:**
- Parameter optimization using backpropagation in time
- Loss function design for trajectory matching
- Gradient-based optimization algorithms
- Comparison of different optimization approaches for dynamical systems

## Setup Instructions

### Prerequisites
- Python 3.7 or higher
- pip package manager

### Installation

1. **Clone the repository** (if working from a remote source):
   ```bash
   git clone <repository-url>
   cd pytorch_applications
   ```

2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
