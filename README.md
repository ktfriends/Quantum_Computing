# <Comparison of global minimum ratios of QUBO and Ising models>

## Solving linear system
```
Solving linear system: Ax = b
This folder solve the below matrix and vector with 12 qubits
     1   -1    1
A = -2    3    4 , b = (4, -4, 8)
     1   -4   -1
```

## File description
```
QA_12qubits.ipynb: Original QUBO and Ising models
QA_12qubits_penalty.ipynb: QUBO and Ising models with constraint terms equal to 0
QA_12qubits_penalty.ipynb: QUBO and Ising models with constraint terms equal to 1000
QA_12qubits_rmvd_penalty.ipynb: QUBO and Ising models with removed constraint terms
```

## Success rate finding global minimum (10,000 anneals)
```
                Original        Panelty 0        Panelty 1,000    Panelty removed
QUBO                  57         299, 279              67, 278           508, 605
Ising                175         363, 703             176, 114           258, 960
```

# <Sylvester_Theorem Folder>

## Summary
- This folder contains sage & python code for implementing QUBO formulations for system of linear equations using Sylvester's law of inertia.
- Joint work with Sun Woo Park
- The same code can be found in the following link: https://github.com/spark483/Quantum_Computing_sub

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
