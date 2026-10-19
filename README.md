# Grover’s Algorithm with Qiskit

This project, developed as part of a second-year university course, demonstrates Grover’s search algorithm using Qiskit.

Grover’s algorithm searches an unstructured space of possible answers for a marked item. This notebook uses a three-qubit circuit to introduce the algorithm’s main components and run the circuit on a simulator.

## Project contents

- `Grovers_alg_qiskit.ipynb`: notebook that builds and simulates the circuit.
- `Grovers_algorithm.pdf`: theoretical overview of the algorithm and the quantum physics principles behind it. *(The document is in Italian.)*

## How it works

The circuit first prepares a uniform superposition of the possible states. It then repeats two operations for the calculated number of iterations:

1. **Phase oracle**: marks the solution by changing its phase.
2. **Diffuser**: amplifies the probability of measuring the marked state.

Finally, measurement converts the quantum state into a classical result. The notebook runs the circuit with Qiskit’s `BasicSimulator` and displays the measurement results as a distribution.

## Requirements

- Python
- Qiskit
- Matplotlib
- Jupyter Notebook or JupyterLab

To run the IBM Quantum section, you will also need `qiskit-ibm-runtime`, a configured IBM Quantum account, and access to the backend specified in the notebook.

## Running the notebook

Open `Grovers_alg_qiskit.ipynb` in Jupyter and run the cells in order. The `BasicSimulator` section runs locally and does not require access to a quantum device. The IBM Quantum section is optional.

