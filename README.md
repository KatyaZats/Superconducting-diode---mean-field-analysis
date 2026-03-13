This repository contains numerical simulations developed during my PhD
research on superconducting diode effect in Josephson junctions.

There are two notebooks:

- **MFA_no_bbath_l=2_multvar.ipynb** implements the multivariable mean-field self-consistency loop for the case of orbital number l=2, with spin-orbit intreaction and Zeeman field,
without the coupling to the external bosonic bath.
- **MFA_with_bbath_mult_var_l=2.ipynb** implements the multivariable mean-field self-consistency loop for the case of orbital number l=2, with spin-orbit intreaction and Zeeman field,
  including the coupling to the external bosonic bath. Inclusion of the external bosonic bath induces transitions between the fermionic (Andreev states and continuum states) and requires
  solving the Lindblad equation - here in the form of the many-body steady state.

Note: *The code is a work in progress and mainly intended for experimentation!* The mean-field self-consistency loop may require parameter tuning
to achieve convergence for certain regimes. The implementation here
demonstrates the numerical workflow used in the project.

In each notebook, the workflow is the following:
1. Computing single-particle states of the quantum dot with spin–orbit interaction.
2. Constructing the effective Hamiltonian.
3. Calculating Andreev bound state energies.
4. Solving mean-field self-consistency equations.
5. Computing the Josephson current.
