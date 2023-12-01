---
title: "Data from: The role of mutation bias in adaptive molecular evolution: insights from convergent changes in protein function"
doi: 10.5061/dryad.2256f38
referralUrl: https://datadryad.org/stash/dataset/doi:10.5061/dryad.2256f38
categories:
- Dataset
tags:
- Zonotrichia capensis
- Merganetta armata
- Selasphorus platycercus
- Pterophanes cyanopterus
- Boissonneaua matthewsii
- Periparus ater aemodius
- Lophonetta specularioides alticola
- Hydropsalis longirostris
- Aglaeactis castelnaudii
- Colibri coruscans
- Aegithalos bonvaloti
- Anas cyanoptera orinoma
- Lophonetta specularioides specularioides
- Eriocnemis luciani
- High Altitude
- Metriopelia melanoptera
- Lophophanes dichrous
- Chalcostigma stanleyi
- Hemoglobin
- Conirostrum cinereum
- Poecile palustris
- Schistes geoffroyi
- FOS: Biological sciences
- Cinclodes albiventris
- Coeligena violifer
- Parus minor
- Oreotrochilus estella
- Diglossa glauca
- Chalcostigma ruficeps
- Anas georgica
- Coeligena coeligena
- Troglodytes aedon
- Anser anser
- Catamenia analis
- Heliodoxa leadbeateri
- Cyanochen cyanoptera
- Anairetes nigrocristatus
- Anser indicus
- Chloephaga melanoptera
- Hydropsalis descussata
- Pygochelidon cyanoleuca
- Anas flavirostris oxyptera
- Haplophaedia aureliae
- Amazilia amazilia
- Anas versicolor
- Anas flavirostris flavirostris
- Neochen jubata
- protein evolution
- Columbina cruziana
- Anas puna
- Pteronetta hartlaubi
- Notiochelidon murina
- Adelomyia melanogenys
- Archilochus alexandri
- Anairetes reguloides
- Furnarius leucopus
- Spinus magellanicus
- Parus humilis
- Diglossa brunneiventris
- Periparus ater pekinensis
- Tangara nigroviridis
- Oxyura jamaicensis
- Aegithalos fuliginosus
- Anas cyanoptera cyanoptera
- Amazilia viridicauda
- CpG
- Mutation bias
- Tangara vassorii
publishers:
- Dryad
author:
- Storz, Jay F.
- Natarajan, Chandrasekhar
- Signore, Anthony V.
- Witt, Christopher C.
- McCandlish, David M.
- Stoltzfus, Arlin
affiliations:
- National Institute of Standards and Technology
- University of New Mexico
- University of Nebraska - Lincoln
- Cold Spring Harbor Laboratory
funders:
- National Science Foundation
---

# Abstract
An underexplored question in evolutionary genetics concerns the extent to which mutational bias in the production of genetic variation influences outcomes and pathways of adaptive molecular evolution. In the genomes of at least some vertebrate taxa, an important form of mutation bias involves changes at CpG dinucleotides: If the DNA nucleotide cytosine (C) is immediately 5’ to guanine (G) on the same coding strand, and if the C is methylated, then C→T and G→A mutations occur at an elevated rate relative to mutations at non-CpG sites. Here we examine experimental data from case studies in which it has been possible to identify the causative substitutions that are responsible for adaptive changes in the functional properties of vertebrate hemoglobin (Hb). Specifically, we examine the molecular basis of convergent increases in Hb-O2 affinity in high-altitude birds. Using a data set of experimentally verified, affinity-enhancing mutations in the Hbs of highland avian taxa, we tested whether causative changes are enriched for mutations at CpG dinucleotides relative to the frequency of CpG mutations among all possible missense mutations. The tests revealed that a disproportionate number of causative amino acid replacements were attributable to CpG mutations, demonstrating that mutation bias can influence outcomes of molecular adaptation.

## TechnicalInfo
README for supplementary data from Storz, et al. This is the main README file for the supplementary data package for the study of CpG bias in avian hemoglobin adaptation by Storz, et al., entitled "The role of mutation bias in adaptive molecular evolution: insights from convergent changes in protein function" (10.1098/rstb.2018.0238). # EXPLANATION Based on prior work, Storz, et al. provide a summary of experimentally validated changes in hemoglobin affinity associated with altitude adaptation in 35 pairs of closely related low- and high-altitude bird populations. The authors report on a statistically significant association of CpG mutation hotspots with these adaptive changes. This supplementary data package provides a script and data files that reproduce the main results by processing the primary data, recomputing the null expectations, and conducting statistical tests. The data also may be useful to researchers carrying out meta-analyses of cases in which adaptation can be traced to specific molecular changes. # DESCRIPTION OF FILES The files are all text files, including sequence alignment files in FASTA format, tables in csv (comma-separated values) format, and an R-MarkDown script: * altitude_pairs_changes_2018-09-13.csv (primary data file describing validated changes) * altitude_pairs_changes_meta.csv (data definition file for above) * hb_CpG_analysis.Rmd (script to process data, calculate null models, carry out tests) * alpha-globin_ancestral_seqs.fas (reconstructed ancestral Hb alpha A sequences) * beta-globin_ancestral_seqs.fas (reconstructed ancestral Hb beta sequences) * README.txt (this file) # HOW TO OBTAIN THE CONTENTS The contents of this package are available from Dryad () or from the authors (see TECHNICAL SUPPORT). # SOFTWARE REQUIREMENTS The files are all text files readable with a text editor. The csv (comma-separated values) files can be opened with Excel and a variety of other tools. The script is written in R-markdown and is best used in RStudio. The code chunks in the Rmd file also can be copied and pasted into an R environment. # VALIDATION The hb_CpG_analysis.Rmd script will generate script_output/altitude_pairs_obs_exp.csv (null expectations and counts) and script_output/test_results.csv (P values). The contents of these files can be compared with values reported in the manuscript. Use the following assertions to validate the integrity of the files and the correctness of processing without the Rmd script: * each FASTA file has exactly 35 ancestral CDS sequences, one for each pair * there are no gaps in the sequences * the main data file describes 10 paths with 6, 3, 3, 2, 2, 2, 1, 1, 1, 1 events * there are 6 G to S (Gly to Ser) changes at site 83 in HBB * the HBA change from A to V at site 63 is in a CpG context * the HBA change from P to A at site 119 is not in a CpG context # TECHNICAL SUPPORT For questions about data processing and statistical analysis, contact Arlin Stoltzfus (). For questions about experimental data and natural history of the bird species, contact Jay Storz (). # STATEMENT OF RIGHTS AND DISCLAIMER The authors release the data and scripts in this package into the public domain, with no warranty, under a Creative Commons Zero (CC0 1.0) license.

# Access Points
https://datadryad.org/stash/dataset/doi:10.5061/dryad.2256f38

# Related Identifiers
## IsCitedBy
- https://doi.org/10.1098/rstb.2018.0238
## IsDerivedFrom
- https://doi.org/10.5281/zenodo.10198318