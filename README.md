# Introduction to Quantum Computing with Qiskit and QuTiP

This repository contains a Jupyter Notebook introducing the fundamentals of quantum computing through hands-on examples using **Qiskit** and **QuTiP**.

The notebook explores three main topics:

- **Quantum circuits with Qiskit:** Building quantum circuits, applying quantum gates, and visualizing circuit operations.
- **Grover's algorithm:** Implementing a four-qubit Grover search algorithm, understanding the oracle and diffusion operator, and running the circuit on a quantum simulator.
- **Qubit visualization with QuTiP:** Representing qubit states on the Bloch sphere and visualizing how quantum states evolve under successive quantum operations.

## 1. Requirements and installation

Make sure you have Python 3.10 or later installed.

Install the required packages:

```bash
pip install qiskit qiskit-aer qutip matplotlib numpy jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and run the cells sequentially.

## 2. Running quantum circuits on a simulator

The notebook uses **Qiskit Aer** to simulate quantum circuits locally, without requiring access to quantum hardware.

The Aer simulator is installed through:

```bash
pip install qiskit-aer
```

You can execute circuits using the `AerSimulator` backend provided by Qiskit Aer.

## 3. Running circuits on real quantum hardware

To execute circuits on IBM Quantum hardware, you need an IBM Quantum account and the Qiskit IBM Runtime package.

Install the package:

```bash
pip install qiskit-ibm-runtime
```

Create an account on [IBM Quantum Platform](https://quantum.ibm.com/) and generate an API key.

Configure your IBM Quantum account using:

```python
from qiskit_ibm_runtime import QiskitRuntimeService

QiskitRuntimeService.save_account(
    channel="ibm_quantum_platform",
    token="YOUR_API_KEY",
    overwrite=True
)
```

You can then access available quantum backends and submit circuits for execution using Qiskit IBM Runtime.

**Note:** Real quantum hardware access depends on your IBM Quantum account, available backends, and current service access policies.

## 4. Qubit visualization with QuTiP

The notebook also uses **QuTiP (Quantum Toolbox in Python)** to represent and visualize single-qubit states.

QuTiP provides tools for quantum-state representation, quantum dynamics, and visualization, including Bloch sphere representations.

Installation:

```bash
pip install qutip
```

## 5. Repository structure

```text
.
├── intro-to-QC-AQC-workshop-26.ipynb
└── README.md
```

## Acknowledgements

Built using:
- [Qiskit](https://www.ibm.com/quantum/qiskit)
- [Qiskit Aer](https://github.com/Qiskit/qiskit-aer)
- [QuTiP](https://qutip.org/)


