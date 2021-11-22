# <Sylvester_Theorem Folder>

## This folder contains sage & python code for implementing QUBO formulations for system of linear equations using Sylvester's law of inertia.

## Matrix_congruence_update.ipynb
### This calculator prints out the d-wave quantum annealer command for solving a system of linear equations using the quadratic unconstrained binary optimization formulation. 

## QA_X-qubits.ipynb
### The following code implements the following QUBO models which utilize X qubits.
#### QUBO formulation utilizing Sylvester's law of inertia & qubit relations (compiles up to 132 qubits)
#### QUBO formulation utilizing only the quadratic relation q^2 = q (compiles up to 64 qubits)
#### (The error message "no embedding found" shows that the D-wave quantum annealer cannot process the second QUBO formulation.)
