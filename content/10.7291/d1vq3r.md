---
title: "FEHM source code modifications and executables for use with ocean-world gravity"
doi: 10.7291/d1vq3r
referralUrl: https://datadryad.org/stash/dataset/doi:10.7291/D1VQ3R
categories:
- Dataset
tags:
- Seafloor
- Europa
- Planetary sciences
- Ocean worlds
- hydrothermal
- Enceladus
- FEHM
- FOS: Physical sciences
- Numerical Simulation
publishers:
- Dryad
author:
- Fisher, Andrew
- Dickerson, Kristin
- Blackman, Donna
- Randolph-Flagg, Noah
- German, Christopher
- Sotin, Christophe
affiliations:
- Blue Marble Space Institute of Science
- University of California, Santa Cruz
- University of Nantes
- Woods Hole Oceanographic Institution
sponsor:
- University Of California, Santa Cruz
funders:
- National Aeronautics and Space Administration
- National Science Foundation
---

# Abstract
This is a repository for compiled codes, source code, and input files used in this paper: Fisher, A. T., K. D. Dickerson, D. K. Blackman, N. Randolph-Flagg, C. R. German, and C. Sotin (2024), Sustained hydrothermal circulation under ocean-world gravity, J. Geophys. Res. - Planets, submitted and in review. Plain language summary from paper: Ocean worlds are planets, moons, and other rocky bodies that have a liquid ocean, often under an icy shell or within the rocky interior. In our solar system, ocean worlds include several moons of Jupiter and Saturn. Some of these ocean worlds are thought to have active hydrothermal circulation, where water, rocks, and heat combine to drive fluids in and out of the seafloor. Hydrothermal circulation could impact the chemistry of the water, rock, and ice of ocean worlds and provide chemical energy that allows life to develop deep below the icy surface. This study shows results from computer simulations of hydrothermal circulation, using a well-understood system on Earth as the basis for comparison to conditions on an ocean world that has much lower gravity (because it is smaller than Earth). The simulations show that fluid flow much like that occurring at seafloor sites on Earth could occur under ocean world gravity, but with several important differences. Lower gravity results in less buoyancy, where warmed fluid expands and becomes lighter than nearby cold fluid. Less buoyancy tends to reduce flow rates in a hydrothermal system, and this can result in higher temperatures of the circulating fluid, and more extensive chemical reactions. Lower gravity can also result in hydrothermal systems transporting less heat, and this could allow these systems to last longer on an ocean world.

## Methods
There is a README file with information on files posted, and a Supporting Information document that goes with the paper that discusses modifications to code in some detail. The main research paper also discussed how the code was used.

## TechnicalInfo
FEHM source code modifications and executables for use with ocean-world gravity FEHM archive for Fisher et al. (202X), "Sustained hydrothermal circulation under ocean-world gravity," in preparation for submission to Journal of Geophysical Research - Planets. [above will be revised when paper review is completed, and a DOI will be added for the final version, when it is published.] ## Description of the data and file structure Three compressed (zip) files are included in this archive: 10_FEHM-Linux_Diffg_Exe.zip 20_FEHM-SourceEdited.zip 30_FEHM-InputDirs.zip ## Sharing/Access information ## Code/Software #### 10\_FEHM-Linux\_Diffg\_Exe.zip Contains executable FEHM programs with gravity for Earth, Europa, and Enceladus: xfehm_v3.4.01grav Earth xfehm_v3.4.01g1_3 Europa xfehm_v3.4.01g_114 Enceladus These codes were compiled under the CentOS 6 (Linux) operating system using gfortran. #### 20\_FEHM-SourceEdited.zip Contains original and edited subroutines and a Makefile for compiling new versions of FEHm with different gravity values. To use these routines, remove the suffix \_orig or \_edit, edit files as needed, place files in source directory with other subroutines, then recompile with the Makefile. #### 30\_FEHM-InputDirs.zip Example directories are provided for running FEHM to duplicate results shown in Figure 3 of the main paper. This figure shows snapshots of results from four simulations, files for each of which are stored in separate subdirectories: A_p12fto_OCv10_g981 B_p12d1200efto_OCv10_g1_3 C_p12d600efto_OCv10_g1_3r D_p10d600efto_OCv10_g_114 ##### A\_p12fto\_OCv10\_g981 Shallow aquifer, aquifer permeabilty = 1e-12 m^2, Earth gravity ##### B\_p12d1200efto\_OCv10\_g1\_3 Deep-thick aquifer, aquifer permeabilty = 1e-12 m^2, Europa gravity ##### C\_p12d600efto\_OCv10\_g1\_3r Deep-thin aquifer, aquifer permeabilty = 1e-12 m^2, Europa gravity ##### D\_p10d600efto\_OCv10\_g\_114 Deep-thin aquifer, aquifer permeabilty = 1e-10 m^2, Enceladus gravity In addition to the input files in each directory, the user will need to copy over or add a static link for the fluid properties lookup table, nist120-1800.out, and update the name in the .files file to point to this table. Please see the FEHM User Manual for more detailed instructions for use of FEHM, available with the GitHub repository: Code modifications included in this repository are covered by the FEHM license, as described in the associated README file.

# Access Points
https://datadryad.org/stash/dataset/doi:10.7291/D1VQ3R

# Related Identifiers
## IsDerivedFrom
- https://doi.org/10.5281/zenodo.10085817
## IsSourceOf
- https://doi.org/10.5281/zenodo.10085825