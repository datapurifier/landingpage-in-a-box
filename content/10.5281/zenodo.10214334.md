---
title: "Kinoson data for FCC random and high entropy alloys"
doi: 10.5281/zenodo.10214334
referralUrl: https://zenodo.org/doi/10.5281/zenodo.10214334
categories:
- Dataset
publishers:
- Zenodo
author:
- Trinkle, Dallas
- Chattopadhyay, Soham
affiliations:
- University of Illinois System
- University of Illinois Urbana-Champaign
funders:
- National Science Foundation
---

# Abstract
This database contains the single KMC-step datasets for the "Ordered" and "Random" rate lattice gas systems, as well the "Complex" high-entropy alloy to accompany our main publication along with our code repository mentioned therein. The datasets are given as HDF5 files, readable with the `h5py` module in python 3. These files are listed below:
* CrystalData: `CrystData.h5` and `CrystData_ortho_5_cube.h5` contain all the necessary FCC crystal structure data for primitive 8x8x8 and orthogonal 5x5x5 FCC supercells.
* Lattice_gas/2-component/Ordered_rate: `singleStep_FCC_SR2_c0_X_Run2.h5` are the datasets for the 2-component "Ordered" rate lattice gas systems
* Lattice_gas/2-component/Random_rate: `singleStepFCC_CR2_c0_X_Run_3.h5` are the datasets for the 2-component "Random" rate lattice gas systems, with X = 60, 70, 75, 80, 85 for the slow species concentration. In these datasets, the slow and fast species have integer labels of 0 and 1, and the vacancy has an integer label of 2.
* Lattice_gas/5-component/Ordered_rate: `singleStep_FCC_5comp_LG_EquiComp_T.h5` are the datasets for the 5-component "Ordered" rate lattice gases
* Lattice_gas/5-component/Random_rate: `singleStep_HEA_dist_EquiComp_T.h5` are the datasets for the 5-component "Random" rate lattice gases, with T = 1073, 1173, 1273, 1373 for the simulated temperatures. In these datasets, the four slow species have integer labels 0, 1, 2 and 3, while the fast species has an integer label of 4, and the vacancy has an integer label of 5.
* HEA_MEAM: `singleStep_HEA_MEAM_T_ftol_1e-3.h5` (T = 773, 1073, 1173, 1273, 1373) contain the single KMC step samples for the complex high-entropy alloy simulated with the MEAM potential. In these datasets, the vacancy has an integer label of 0, while Co, Ni, Cr, Fe and Mn have integer labels 1, 2, 3, 4 and 5.
Along with the datasets, in each directory, the optimal neural network models for each system have also been provided as PyTorch "state dictionaries", along with the optimal neural network-predicted relaxation vectors. To illustrate the use of these datasets, neural networks and their relaxation vectors, python 3 Jupyter notebooks have also been provided to show the calculation of the transport coefficients using the Scaled Bias Basis (SBB) Method for all systems, as well as the NN+SRBC method for the "Complex" high-entropy alloy. In each directory, these notebooks have been numbered in their file names so as to make it easier to navigate through them. Along with such examples and the datasets, source codes for our neural network models and cluster expansion models are available in the code repository mentioned in our main text. Modules in this repository are also required to run these example notebooks.
 

# Access Points
https://zenodo.org/doi/10.5281/zenodo.10214334

# Related Identifiers
## IsVersionOf
- [10.5281/zenodo.10214333](../../10.5281/zenodo.10214333/)