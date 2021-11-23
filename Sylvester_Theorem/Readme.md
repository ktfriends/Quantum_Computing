# <Sylvester_Theorem Folder>

## Summary
- This folder contains sage & python code for implementing QUBO formulations for system of linear equations using Sylvester's law of inertia.
- Joint work with Sun Woo Park
- The same code can be found in the following link: https://github.com/spark483/Quantum_Computing_sub
- Arxiv preprint link: https://arxiv.org/abs/2111.10084

## Matrix_congruence_update.ipynb
- This calculator prints out the d-wave quantum annealer command for solving a system of linear equations using the quadratic unconstrained binary optimization formulation. 

## QA_X-qubits.ipynb
- The following code implements the following QUBO models which utilize X qubits.
  + QUBO formulation utilizing Sylvester's law of inertia & qubit relations (compiles up to 132 qubits)
  + QUBO formulation utilizing only the quadratic relation q^2 = q (compiles up to 64 qubits)
  + (The error message "no embedding found" shows that the D-wave quantum annealer cannot process the second QUBO formulation.)
- QUBO model utilizing Sylvester's Theorem:
  + Empirical maximum number of utilizable qubits: 132 qubits (D-wave 2000Q quantum annealer)
  + Models utilizing more than 136 qubits cannot be compiled (D-wave 2000Q quantum annealer)
- QUBO model utilizing only the quadratic relation:
  + Empirical maximum number of utilizable qubits: 64 qubits (D-wave 2000Q quantum annealer)

