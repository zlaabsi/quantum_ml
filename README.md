# Quantum Machine Learning

## Quantum Gradient Descent

How to train quantum circuit-based models using gradient based methods ?

The goal in the case of classical models is to minimize the cost or loss function which is the objective function via the vector of parameters $\vec{\theta}$. In the case where we train a parameterized quantum circuit model, the function to minimize is the expected value $\langle \Psi(\vec{\theta}) \mid \hat{H} \mid \Psi(\vec{\theta})\rangle$ with $\hat{H}$ the Hamiltonian operator defined by the Schrödinger equation $$i\hbar \frac{d|\Psi(\vec{\theta})\rangle}{d\theta} = \hat{H} |\Psi(\vec{\theta})\rangle $$

The expectation value is what we’d expect to measure if we averaged out a large number of results.

The quantum approach has two fundamental steps :

1. Prepare the quantum state $|\Psi(\vec{\theta})\rangle$ called the *ansatz*
2. Measure the expectation value $\langle\,\Psi(\vec{\theta})\,|\,\hat{H}\,|\,\Psi(\vec{\theta})\,\rangle$

We define our ansatz $|\Psi(\vec{\theta})\rangle = U(\vec{\theta})|0\rangle$ with $U(\vec{\theta})$ the parametrized quantum circuit.

<img src="https://latex.codecogs.com/svg.image?$|\Psi(\vec{\theta})\rangle&space;=&space;U(\vec{\theta})|0\rangle$&space;" title="$|\Psi(\vec{\theta})\rangle = U(\vec{\theta})|0\rangle$ " />

<img src="https://latex.codecogs.com/png.image?\dpi{110}&space;$|\Psi(\vec{\theta})\rangle&space;=&space;U(\vec{\theta})|0\rangle$&space;" title="$|\Psi(\vec{\theta})\rangle = U(\vec{\theta})|0\rangle$ " />
