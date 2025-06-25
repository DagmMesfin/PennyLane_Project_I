# PennyLane Tasks of iCog Labs Training

## Overview
This project explores various quantum computing tasks using PennyLane, a Python library for quantum machine learning, quantum chemistry, and quantum computing. The tasks are designed to provide hands-on experience with quantum circuits, measurements, and optimization techniques.

## Tasks

### Task 1: Create a Bell State Circuit
- **Objective**: Build a quantum circuit that generates the Bell state.
- **Details**:
  - Use 2 qubits.
  - Display the probability distribution using `qml.probs()`.
  - Bonus: Visualize the statevector or show measurement samples.

### Task 2: Build a GHZ State for 3 Qubits
- **Objective**: Construct a circuit that prepares a 3-qubit GHZ state.
- **Details**:
  - Use Hadamard and CNOT gates.
  - Measure using `qml.probs(wires=[0, 1, 2])`.
  - Optional: Extend to 4 qubits.

### Task 3: Rotation + Measurement Circuit
- **Objective**: Design a single-qubit rotation circuit using RX, RY, or RZ gates.
- **Details**:
  - Make the rotation angle a variable input.
  - Return the expectation value of PauliZ.
  - Plot how the output changes as you vary the input angle.

### Task 4: Simple Variational Optimization
- **Objective**: Create a cost function that depends on a gate parameter and optimize it using PennyLane’s gradient descent optimizer.
- **Details**:
  - Use a rotation gate like RX and minimize `expval(PauliZ)`.
  - Log or print the cost at each step.
  - Output the optimal parameter found.
  - Plot the cost function curve.

### Task 5: Measurement Comparison
- **Objective**: Build a 1- or 2-qubit circuit and compare results from different measurement methods.
- **Details**:
  - Compare `qml.probs()`, `qml.sample()`, and `qml.expval()`.
  - Explain how they differ in output and when to use each.
  - Discuss why `qml.probs()` is deterministic but `qml.sample()` is random.

## Requirements
- Python 3.x
- PennyLane
- Matplotlib
- NumPy

## Installation
Follow these steps to set up the project:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/DagmMesfin/PennyLane_Project_I.git
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install the Requirements**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Open the Notebook**:
   Launch Jupyter Notebook and open the `PennyLane_Task.ipynb` file located in the `notebooks` directory.
   
## License
This project is licensed under the MIT License.