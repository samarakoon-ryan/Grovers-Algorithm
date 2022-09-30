# Implementation of Grover's Algorithm using Qiskit

## Introduction

Grover's algorithm demonstrates the possibility of superior searching capabilities when used with a quantum computer. The algorithm is able to speed up an unstructured search problem quadratically. On a quantum computer, given a list of N items, we can find a marked item in $\sqrt{N}$ time. Grover's algorithm uses a diagonal matrix as the oracle, where the entry that corresponds to the marked item will have a negative phase.

## Algorithm

1. Amplitude amplification procedure
2. Apply the oracle reflection to the state
3. Apply an additional reflection about the state
4. Step 2 & 3 are repeated as this transformation continues to boost the negative amplitude of the marked item and decreases the other amplitudes. This is repeated roughly $\sqrt{N}$ times.

## Implementation

I've implemented an example using 2 qubits searching for |11> using Qiskit in an iPython notebook. A more thorough explanation of the algorithm is commented in the notebook `implementation.ipynb`. After implementation and experiment is ran with a simulator and a real device.
