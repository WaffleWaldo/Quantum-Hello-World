# 'Hello World'

This project demonstrates how to use Qiskit to create and run a simple quantum circuit on both a local simulator and a real quantum computer.

## Installation

To run this project, you will need to have Qiskit installed. You can install it using pip:

```pip install qiskit```

You will also need to install matplotlib and qiskit-ibm-provider for visualization and using the IBM quantum computer:

```pip install matplotlib```
```pip install qiskit-ibm-provider```

## Usage

The code defines a quantum circuit that applies the Hadamard gate to the first qubit and then performs a controlled-NOT (CX) gate on both qubits. Finally, the circuit measures both qubits and stores the results in classical registers.

![](assets/H%20Gate.png)

To run the circuit on a local simulator, simply execute the code in a Python environment:

```python quantum_circuit.py```

This will display the circuit diagram and a histogram of the measurement results.

![](assets/Histo%20Sim.png)

To run the circuit on a real quantum computer, you will need to have an IBM Quantum Experience account and API key. Replace `"ibm-q/open/main"` with your desired backend and `your_api_key` with your actual API key in the following line:

```provider = IBMProvider(token='your_api_key', instance="ibm-q/open/main")```

Then, execute the code and run the circuit on the chosen backend:

```python quantum_circuit.py```

![](assets/Histo%20Quantum.png)

This will display the circuit diagram and a histogram of the measurement results, as well as submit the job to the backend and monitor its progress. Once the job is complete, the histogram of the actual results obtained from the quantum computer will be displayed.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.


