# Comparison of global minimum ratios of QUBO and Ising models

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
