# Optimized Model: Evolution of Cosmological Magnetic Fields
Author: Giovannimaria Grillo
Date: 02/02/2025
## Description

This repository contains the code, data, and documentation for the **Revised Optimized Model** developed to study the evolution of cosmological magnetic fields. The model integrates multiple modules:
- **Subgrid Module:** Models turbulent amplification on sub-kiloparsec scales using an LES-MHD approach.
- **Astrophysical Feedback Module:** Implements a nonlinear model for feedback from events such as supernovae and AGN jets.
- **Reconnection Module:** Uses a hybrid approach combining MHD corrections with PIC 3D simulations, including an extension into ultra-relativistic regimes (UltraUltraRel).
- **Advanced Chemical Module:** Incorporates a chemical network that accounts for H, He, H₂, metals, and dust, further updated to integrate even more complex molecular reactions (e.g., formation/destruction of complex molecules) to better represent conditions in extreme environments and at high redshift.

The model has been rigorously validated through convergence tests, benchmarking, sensitivity analyses, and comparisons with observational data (e.g., Faraday rotation and polarization maps).

## Requirements

- **Compilers/Interpreters:** 
  - C/C++/Fortran (if using compiled code)
  - Python 3.x (if using Python scripts)
- **Dependencies:** MPI, OpenMP, BLAS, LAPACK, NumPy, SciPy, Matplotlib, etc.
- **Additional tools:** Git (for version control) and an HPC environment for large-scale simulations.

## Installation

Install Dependencies:

For Python, install the required packages using:
pip install -r requirements.txt
For compiled languages, follow the instructions in INSTALL.md.
Compile the Code (if necessary):
Run:
make
or follow the instructions in INSTALL.md.

How to Run
To run an example simulation, you can use the provided script:
Using Bash Script:
bash examples/run_simulation.sh
Using Python:
python code/main.py --config config/simulation_config.json
Simulation outputs will be stored in the data/simulation_results/ directory.

Replication Guide
For a detailed explanation on how to replicate the model, please refer to the Replication Guide. This guide covers:

Setting up the computational environment.
Detailed configuration of simulation parameters.
Step-by-step instructions for running simulations and analyzing data.
User Manual
A comprehensive user manual is available in the User Manual, which includes:

An overview of the model architecture.
A description of each module (Subgrid, Feedback, Reconnection, and Chemical Network).
Detailed instructions on how to interpret simulation results.
