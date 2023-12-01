---
title: "Foraging behavior of tagged rock ants (Temnothorax rugatulus)"
doi: 10.5061/dryad.xksn02vn0
referralUrl: https://datadryad.org/stash/dataset/doi:10.5061/dryad.xksn02vn0
categories:
- Dataset
tags:
- Temnothorax
- recruitment
- T. rugatulus
- Tandem running
- FOS: Natural sciences
publishers:
- Dryad
author:
- Taylor, Benjamin
- Rajagopal, Supraja
- Sasaki, Takao
affiliations:
- University of Georgia
funders:
- National Science Foundation
- University of Georgia
---

# Abstract
Technological advances continue to push the boundaries of scientific inquiry in animal behavior. One such development is the emergence of automated tracking systems, which enable the collection of high-resolution spatio-temporal information for animals. Although tag-based tracking systems provide valuable insights into animal movement and collective behavior, the attachment of devices can have detrimental effects in some cases. Here, we investigated the effects of recently developed miniature tracking tags using the rock ant, Temnothorax rugatulus, as a model system. To do so, we compared the foraging activities of tagged ants and untagged ants (who lost their tags) within initially fully-tagged colonies. Additionally, we compared the foraging activities of these initially fully-tagged colonies with those of no-tag control colonies (no one was tagged). We found that tags did not significantly reduce individual activity, with tagged ants visiting the food source as frequently as untagged ants within initially fully-tagged colonies. However, our analysis revealed a marked difference in recruitment behavior—tagged ants were less likely to participate in tandem runs than untagged ants. Furthermore, the number of tandem runs was higher for the no-tag control colonies than the initially fully-tagged colonies, in which 69–95% of colony members had tags. Our data suggest, for the first time, that tracking tags can negatively impact ant behavior. Although tracking devices are powerful tools for understanding complex behavioral patterns, it is crucial to carefully consider their potential impact on animal behavior to ensure accurate conclusions.

## Methods
Three colonies of ants were tagged prior to foraging experiments (Initially Fully-Tagged: 'R2119', 'R2111', and 'R2100'). However, the final proportion of tagged individuals varied since tags were frequently detached during grooming and handling. Three colonies were never tagged and served as control groups (Not-tagged: 'FR2217', 'FR2218', and 'FR2220'). For 5 hours and 30 minutes, we annotated videos (S1 Video Repository), recording the status (column: "tag_status") of each ant ("tagged" or "untagged") and time of occurrence for three foraging events: Feeding at food source ("Feeder visit") Leading a tandem run ("Tandem-running leader") Following a tandem run ("Tandem-running follower")

## Other
All statistical analyses were performed in Python with the SciPy and Statsmodels. A complete list of our Python environment and all dependencies is included: "env-specs.yml."

## TechnicalInfo
Foraging behavior of tagged ants dataset *** Authors: [Ben Taylor](mailto:benjaminztaylor@gmail.com), Supraja Rajagopal, and Takao Sasaki *** Three colonies of ants were tagged prior to foraging experiments (**Initially Fully-Tagged**: 'R2119', 'R2111', and 'R2100'). However, the final proportion of tagged individuals varied since tags were frequently detached during grooming and handling. Three colonies were never tagged and served as control groups (**Not-tagged**: 'FR2217', 'FR2218', and 'FR2220'). For 5 hours and 30 minutes, we annotated videos ([S1 Video Repository](https://kaltura.uga.edu/playlist/dedicated/1_dsklo3z0/1_4yj44wyy)), recording the status ("tag\_status") of each ant ("tagged" or "untagged") and time of occurrence for three foraging events: 1. Feeding at food source ("Feeder visit") 2. Leading a tandem run ("Tandem-running leader") 3. Following a tandem run ("Tandem-running follower") ## **Description of the data and file structure** ### File: `colony_information.csv` **Description**: This file contains basic details details regarding the count of tagged and untagged ants in each colony. #### Details * `Colony`: Colony identity (*str*) * `Whole colony_Tagged`: the number of ants with tags in the colony (*int*) * `Whole colony_Untagged`: the number of ants within a colony that do not have tags (*int*). **Note**: For "Initially fully-tagged" colonies "untagged" describes ants that were formerly tagged. *** ### File: `foraging_behavior_data.csv` **Description**: This file contains annotations of foraging events for all colonies. Each row represents a unique feeder visit, detailing the following attributes: #### Details * `colony`: Colony identity (*str*) * `colony_treatment`: Treatment type applied to the colony ("Not-tagged" *or* "Initially fully-tagged") * `behavior`: Specifies the behavior observed during the event. It designates whether the ant is a "Feeder visit", "Tandem-running leader" or a "Tandem-running follower." (*str*) * `time`: Video timestamp indicating the time of the event.(*datetime64*) * `tag_status`: Tag status of the ant involved in the foraging event. (*str*) **Note**: This dataset only includes records of successful tandem runs. For information on both successful and unsuccessful tandem runs, refer to the `all_tandem_run_behavior.csv` data. *** ### File: `all_tandem_run_behavior.csv` **Description**: This dataset contains records of all tandem running behaviors, encompassing both successful and unsuccessful runs. An unsuccessful tandem run occurs when recruitment is initiated but the pair fails/breaks to reach the target food source. #### Details * `colony`: Colony identity (*str*) * `colony_treatment`: Treatment type applied to the colony ("Not-tagged" *or* "Initially fully-tagged") (*str*) * `successful`: Indicates if the tandem run was successful (1) or unsuccessful (0) (*int*) * `tr_start`: Timestamp of tandem behavior start (*datetime64*) * `tr_end`: Timestamp of tandem behavior end (*datetime64*) * `tr_leader_tag_status`: Tag status of the tandem run leader (*str*) * `tr_follower_tag_status`: Tag status of the tandem run follower (*str*) ## **Sharing/Access information** **S1 Video Repository**: Videos of foraging experiments for each colony can be accessed via Kaltura video repository: [Access Here](https://kaltura.uga.edu/playlist/dedicated/1_dsklo3z0/1_4yj44wyy). ## **Code/Software** All statistical analyses were conducted in Python. `Tag_attachment_reduces_initiation_stats.ipynb`: Python notebook contain statistical analysis. * Fisher's Exact and T-tests (SciPy) * OLS Regression and S1 Table 1 (Statsmodels) * Fig 3 creation (Plotly) A complete list of our Python environment and dependencies is included in `env-specs.yml.` Replicate our environment with Conda (MacOS): `conda env create -f env-specs.yml`

# Access Points
https://datadryad.org/stash/dataset/doi:10.5061/dryad.xksn02vn0

# Related Identifiers
## IsDerivedFrom
- https://doi.org/10.5281/zenodo.8429080
## IsSupplementedBy
- https://kaltura.uga.edu/playlist/dedicated/1_dsklo3z0/1_4yj44wyy