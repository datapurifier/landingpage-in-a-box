---
title: "Observation of mHz-level cooperative Lamb shifts in an optical atomic clock"
doi: 10.5061/dryad.wpzgmsbtj
referralUrl: https://datadryad.org/stash/dataset/doi:10.5061/dryad.wpzgmsbtj
categories:
- Dataset
tags:
- Lasers
- FOS: Physical sciences
- Atomic ph
- Quantum optics
publishers:
- Dryad
author:
- Hutson, Ross B.
- Milner, William R.
- Yan, Lingfeng
- Ye, Jun
- Sanner, Christian
affiliations:
- Joint Institute for Laboratory Astrophysics
- Colorado State University
funders:
- National Science Foundation
- National Institute of Standards and Technology
- United States Department of Energy
- Vannevar Bush Fellowship
---

# Abstract
We report on the direct observation of resonant electric dipole-dipole interactions in a cubic array of atoms in the many-excitation limit. The interactions, mediated by single-atom couplings to the shared electromagnetic vacuum, are shown to produce spatially-dependent cooperative Lamb shifts when spectroscopically interrogating the mHz-wide optical clock transition in strontium-87. We show that the ensemble-averaged shifts can be suppressed below the level of evaluated systematic uncertainties for state-of-the-art optical atomic clocks. Additionally, we demonstrate that excitation of the atomic dipoles near a Bragg angle can enhance these effects by nearly an order of magnitude compared to non-resonant geometries. Given the remarkable precision of frequency measurements and the high accuracy of the modeled response, our work demonstrates that such a clock is a novel platform for studies of the quantum many-body physics of spins with long-range interactions mediated by propagating photons.

## TechnicalInfo
Observation of mHz-level cooperative Lamb shifts in an optical atomic clock [https://doi.org/10.5061/dryad.wpzgmsbtj](https://doi.org/10.5061/dryad.wpzgmsbtj) The python script "make\_figures.py" produces the plots in Figs. 2-4, S1-S3 given the images and control parameters contained in "cls.h5" ## Description of the data and file structure The data in "cls.h5" is saved in HDF5 format and contains the following datasets * "timestamp\_": array of timestamps corresponding to the (UNIX) time at which the corresponding experimental shot began. * "runpath\_": unique strings distinguishing runs, between which realignment/calibration procedures were performed. * "φ\_": array specifying pulse phases sin(φ\_out) * "Z\_": array specifying initial pulse area 4 sqrt(2) cos(θ\_in) * "q\_": array specifying probed transition * "ψ\_": array specifying angle of incidence * "counts\_g\_": array of ground state images * "counts\_e\_": array of excited state images ## Code/Software Running the python script "make\_figures.py" requires Python 3.11+ and the following third-party libraries: allantools, h5py, matplotlib, numpy, scipy

# Access Points
https://datadryad.org/stash/dataset/doi:10.5061/dryad.wpzgmsbtj