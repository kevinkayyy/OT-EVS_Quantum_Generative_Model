# OT-EVS_Quantum_Generative_Model

This repo contains the official implementation for the paper Shadow-Frugal Expectation-Value-Sampling Variational Quantum Generative Model (arXiv:2412.17039). We demonstrate the training of OT-EVS in controlled experiments on synthetic datasets, as well as on image datasets including MNIST and Fashion-MNIST. Most of the numerical results in the paper can be reproduced based on one of the notebooks. The code can be easily extended for testing applications of the OT-EVS on other customized datasets.

## Installation
To start, you may create a virtual environment with Python 3.11.9 or similar, and install the required packages. 
```bash
python3 -m venv otevs-env
pip install -r requirements.txt
```
Then, you may create a corresponding kernel and open the jupyter notebook.
```bash
python -m ipykernel install --user --name otevs-kernel --display-name "otevs-kernel"
```

## Acknowledgements

We use the package Tensorcircuit for constructing quantum circuits, Equinox for constructing
the remaining architecture of the generator and the critic, Jax for the simulation of training and sampling and
FAISS for the k−NN subroutine in the KLD estimator.

