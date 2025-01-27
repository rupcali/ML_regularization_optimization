# Optimization and Regularization in Deep Learning

This repository includes implementations and analyses of optimization techniques and regularization strategies in deep learning models. The project evaluates the impact of different optimizers, activation functions, and regularization methods on model performance.

---

## Contents

1. **Optimization.ipynb**  
   - Implements and compares various optimization algorithms:
     - **Adam Optimizer**
     - **RMSProp Optimizer**
     - **Momentum Optimizer**
   - Key findings:
     - The combination of ReLU activation with Adam and RMSProp optimizers yielded the highest accuracy.
     - The combination of Sigmoid activation with Momentum showed relatively lower accuracy.

2. **Regularization.ipynb**  
   - Explores the effects of regularization methods (L1 and L2) on the model's accuracy:
     - **L1 Regularization**: Aims to sparsify the weights by setting some to zero.
     - **L2 Regularization**: Penalizes large weights to improve generalization.
   - Key observations:
     - L1 regularization decreased accuracy significantly due to unnecessary feature elimination.
     - L2 regularization was more effective, balancing weight penalties and preserving important features.

3. **Report (PDF)**  
   - Summarizes the experiments and their results, focusing on:
     - Comparisons between activation functions (e.g., Sigmoid vs. ReLU) paired with various optimizers.
     - Regularization techniques and their impact:
       - L1 regularization led to diminished learning capacity by eliminating critical features.
       - L2 regularization performed better by maintaining the model's ability to learn effectively.

---

## Key Results

### Optimizers
- **Best Combinations:**  
  - ReLU + Adam  
  - ReLU + RMSProp  
  These combinations achieved the highest accuracy, demonstrating their suitability for deep and complex neural networks.

- **Insights:** Adam and RMSProp dynamically adjust the learning rate, enabling faster and more accurate model training.

### Regularization
- **L1 Regularization:** Significantly lowered accuracy due to over-penalization of important features.
- **L2 Regularization:** Improved performance by balancing weight magnitudes and preserving critical features.

---

## Requirements

- **Python 3.x**
- **Dependencies:**
  - TensorFlow or PyTorch
  - Matplotlib (for plotting and visualization)
  - NumPy (for numerical computations)
- **Dataset:**  
  - Prepare a dataset suitable for training and testing. (The scripts may need to be updated to incorporate your specific dataset.)

---

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebooks and execute the code:
   ```bash
   jupyter notebook Optimization.ipynb
   jupyter notebook Regularization.ipynb
   ```

---

## References

- This project builds on theoretical and practical insights documented in the accompanying homework report. The experiments and results serve as a guide to understanding optimization and regularization in deep learning.

---

Let me know if you need further updates or additional details!
