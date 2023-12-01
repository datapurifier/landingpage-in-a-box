---
title: "Drought tolerant grassland species are generally more resistant to competition"
doi: 10.5061/dryad.1jwstqk1x
referralUrl: https://datadryad.org/stash/dataset/doi:10.5061/dryad.1jwstqk1x
categories:
- Dataset
tags:
- functional traits
- Community assembly
- plant community dynamics
- population growth rates
- Grasslands
- Resistance to competition
- FOS: Natural sciences
- Drought tolerance
publishers:
- Dryad
author:
- Mount, Hailey
- Smith, Melinda (Mendy)
- Knapp, Alan
- Griffin-Nolan, Robert
- Collins, Scott
- Atkins, David
- Stears, Alice
- Laughlin, Daniel
affiliations:
- Colorado State University
- University of New Mexico
- California State University, Chico
- University of Wyoming
funders:
- United States Department of Agriculture
- National Science Foundation
---

# Abstract
Plant populations are limited by resource availability and exhibit physiological trade-offs in resource acquisition strategies. These trade-offs may constrain the ability of populations to exhibit fast growth rates under water limitation and high cover of neighbors. However, traits that confer drought tolerance may also confer resistance to competition. It remains unclear how fitness responses to these abiotic conditions and biotic interactions combine to structure grassland communities and how this relationship may change along a gradient of water availability. To address these knowledge gaps, we estimated the low-density growth rates of populations in drought conditions with low neighbor cover and in ambient conditions with average neighbor cover for 82 species in six grassland communities across the Central Plains and Southwestern United States. We assessed the relationship between population tolerance to drought and resistance to competition and determined if this relationship was consistent across a precipitation gradient. We also tested whether population growth rates could be predicted using plant functional traits. Across six sites, we observed a positive correlation between low-density population growth rates in drought and in the presence of interspecific neighbors. This positive relationship was particularly strong in grasslands of the northern Great Plains but weak in the most xeric grasslands. High leaf dry matter content and low (more negative) leaf turgor loss point were associated with high population growth rates in drought and with neighbors in most grassland communities. Synthesis: A better understanding of how both biotic and abiotic factors impact population fitness provides valuable insights into how grasslands will respond to extreme drought. Our results advance plant strategy theory by suggesting that drought tolerance increases population resistance to interspecific competition in grassland communities. However, this relationship is not evident in the driest grasslands where aboveground competition is likely less important. Leaf dry matter content and turgor loss point may help predict which populations will establish and persist based on local water availability and neighbor cover, and these predictions can be used to guide the conservation and restoration of biodiversity in grasslands.

## Methods
Cover data These data include a subset of 82 species (113 species-site combinations) that were monitored annually as part of the Extreme Drought in Grasslands Experiment (EDGE). Topographically unform and hydrologically isolated plots were set up across six grassland types (tallgrass prairie, southern mixed-grass prairie, northern mixed-grass prairie, northern shortgrass prairie, southern shortgrass prairie, and desert grassland) and absolute cover of all species in four 1 x 1 m quadrats was estimated yearly from 2012–2017. At each site, ten control plots at each site received ambient rainfall over the experimental period, and ten treatment plots experienced a 66% reduction in growing season precipitation (equivalent to roughly 40–50% over the whole year) using greenhouse rainout shelters equipped with strips of clear corrugated polycarbonate. Additional site and experimental design details are available in Griffin‐Nolan et al., (2019). Population growth rates Percent cover was used as a measure of population size for each species at the quadrat level. Population growth rate at time t was calculated as the total cover of a species in time t+1 divided by the total cover in time t. The natural logarithm of this value (intrinsic rate of increase) for a species in a quadrat describes whether the population increased (positive value) or decreased (negative value) in the transition from year t to t+1. Population growth rates were calculated for each species in each quadrat in each annual transition. Because we use species cover instead of counts of individuals to measure population size, intraspecific cover is equal to the cumulative cover of a species in a quadrat. Interspecific cover in each quadrat is defined as the cumulative cover of all non-focal species in a quadrat. We calculated low-density growth rates for populations of each species at each site to assess fitness in two different conditions: mean neighbor abundance under ambient rainfall and minimum neighbor abundance under extreme drought. Minimum and mean neighbor abundances were averaged across all five years of the experiment. To estimate these growth rates, we fit linear models predicting intrinsic rate of increase for each species in each grassland as a function of drought treatment, intraspecific neighborhood cover, and interspecific neighborhood cover across years. Functional traits Species-level trait data were assembled from several publications and trait databases and these eleven included leaf dry matter content (LDMC; g g-1), average individual leaf area (cm2), leaf turgor loss point (TLP; MPa), leaf nitrogen concentration (%), specific leaf area (SLA; cm2 g-1), leaf tissue density (LTD; cm3 g-1), root nitrogen (%), root tissue density (RTD; cm3 g-1), root diameter (mm), specific root length (SRL; m g-1), and average maximum height (mm). Trait data were compiled for each species at the site level where available (Table S1). Trait values measured at, or nearby, EDGE sites were considered the closest estimate for species traits. For this we used a mix of unpublished and open-access trait data from individual researchers (Blumenthal et al., 2020; Craine et al., 2011; Farrell, 2018; Laughlin et al., 2010; Stears et al., 2022; Tucker, 2010). Grassland communities that did not have data available at the local scale were filled in by progressively broader estimates using regional averages and eventually global estimates provided by the TRY database as needed (Kattge et al., 2019).

## TechnicalInfo
Drought tolerant grassland species are generally more resistant to competition These data were analyzed and presented in the accompanying paper where we observed a positive correlation between low-density population growth rates in drought and low-density population growth rates in the presence of interspecific neighbors. We also found that high leaf dry matter content and low (more negative) leaf turgor loss point were associated with higher population fitness in drought and with higher neighbor competition. The **EDGE_covers.csv** dataset contains aggregated absolute cover estimates and annual population growth summarized from the Extreme Drought in Grassland Experiment (EDGE). The **all_pop_data.csv** contains the calculated population growth rates for each population and the trait data paired with each population. Finally, the **Suppinfo_tableS1_traits.csv** dataset was included as supplemental information for the publication. It also has the population-level traits data but includes details on the sources of trait data and the proximity these measurements were taken to the EDGE population. ## Description of the data and file structure **EDGE_covers.csv** contains 18066 rows where each observation describes the absolute cover of a focal species and the summed absolute interspecific cover of other species present in each unique replicate (subplot). "NA" = not applicable in this dataset. Columns include: * "site" = denotes what site in the EDGE project data is from. CHY = High Plains Grassland Research Station, WY; HYS = Hays Agricultural Research Center, KS; KNZ = Konza Prairie Biological Station, KS; SGS = Central Plains Experimental Range, CO; sev.blue = Sevilleta Wildlife Refuge, NM (shortgrass), sev.black = Sevilleta Wildlife Refuge, NM (desert grassland). * "year" = data was recorded. * "plot" = plot number. * "subplot" = subplot number/ plot replicate number. * "trt" = drought treatment. con = ambient precipitation; chr = 66% reduction in mean annual precipitation. * "species" = Latin names for each species formatted as Genusspecies. * "cover" = absolute cover (%) of the species listed in species column. * "lambda" = population growth rate from the year listed in "year" column to year+1. * "log_lambda" = logged values from "lambda" column to obtain instantaneous rates of increase (r) as growth rate. * "surv" = binary variable used for calculating growth rates. Indicates if a population that was present in the year in the "year" column was still found on the plot in year+1. * "other" = summed absolute cover (%) of all the other species in the subplot excluding the species in "species" column. * "log_cover" = logged values of from "cover" column. * "log_other" = logged values from "other" column. * "cnt" = number of observations of this species across all subplots and years that were used to model population growth rates. **all_pop_data.csv** contains 113 rows where each observation contains the calculated low-density population growth rates in different conditions and trait values for each unique population (species-site combination). "NA" = not available in this dataset. Columns include: * "species" = Latin names for each species formatted as Genusspecies. * "site" = denotes what site in the EDGE project data is from. CHY = High Plains Grassland Research Station, WY; HYS = Hays Agricultural Research Center, KS; KNZ = Konza Prairie Biological Station, KS; SGS = Central Plains Experimental Range, CO; sev.blue = Sevilleta Wildlife Refuge, NM (shortgrass), sev.black = Sevilleta Wildlife Refuge, NM (desert grassland). * "Photosynthesis" = type of photosynthetic pathway. * "annual.Perennial" = lifespan. Includes perennial, annual, and biennial. * "height" = average maximum plant height (mm). * "rootdiam" = root diameter (mm). * "SRL" = specific root length (m g-1). * "RTD" = root tissue density (cm3 g-1). * "rootN" = root nitrogen content (%). * "SLA" = specific leaf area (cm2 g-1). * "LDMC" = leaf dry matter content (g g-1). * "LTD" = leaf tissue density (cm3 g-1). * "leafarea" = leaf area (cm2). * "TLP" = turgor loss point (Mpa). * "leafN" = leaf nitrogen content (%). * "intrinsicLDGRcon" = low density growth rate with 0 interspecific cover in ambient precipitation. * "intrinsicLDGRchr" = low density growth rate with 0 interspecific cover in drought. * "invasionLDGRcon" = low density growth rate with mean interspecific cover in ambient precipitation. * "invasionLDGRchr" = low density growth rate with mean interspecific cover in drought. * "weight" = standard error of models used to calculate low density growth rates. * "weight2" = 1/"weight" column. Used to weight certainty in our growth rates in subsequent models. * "grassland_type" = grassland community type. Includes tallgrass prairie, southern mixed-grass prairie, northern mixed-grass prairie, northern shortgrass prairie, southern shortgrass prairie, and desert grassland. * "grass.forb" = type of growth form grouped into Grass or Other. * "lifespan" = length of species lifespan. grouped into perennial or short-lived species. **Suppinfo_tableS1_traits.csv** contains 186 rows where each observation contains trait data for unique plant populations (species-site combination). Data were compiled from a number of different sources, source author, and location of collection are included and for each population. "NA" = not available, unless noted otherwise below. Columns include: * "Species" = Latin names for each species formatted as Genusspecies. * "grassland" = grassland community type. Includes tallgrass prairie, southern mixed-grass prairie, northern mixed-grass prairie, northern shortgrass prairie, southern shortgrass prairie, and desert grassland. * "site" = denotes what site in the EDGE project data is from. CHY = High Plains Grassland Research Station, WY; HYS = Hays Agricultural Research Center, KS; KNZ = Konza Prairie Biological Station, KS; SGS = Central Plains Experimental Range, CO; sev.blue = Sevilleta Wildlife Refuge, NM (shortgrass), sev.black = Sevilleta Wildlife Refuge, NM (desert grassland). * "grass.forb.shrub" = type of growth form. G = grass; F = forb; S = shrub. * "photosynthesis" = type of photosynthetic pathway. * "annual.perennial" = lifespan. Includes perennial, annual, and biennial. * "max.height (mm)" = average maximum plant height (mm). * "root.diameter (mm)" = root diameter (mm). * "SRL (m g-1)" = specific root length (m g-1). * "root.tissue.density (cm3 g-1)" = root tissue density (cm3 g-1). * "root.nitrogen.content (%)" = root nitrogen content (%). * "SLA (cm2 g-1)" = specific leaf area (cm2 g-1). * "LDMC (g g-1)" = leaf dry matter content (g g-1). * "Leaf.tissue.density (cm3 g-1)" = leaf tissue density (cm3 g-1). * "Leaf.area (cm2)" = leaf area (cm2). * "turgor.loss.point (Mpa)" = turgor loss point (Mpa). * "leaf.nitrogen.content (%)" = leaf nitrogen content (%). * "author_location.primary" = indicates where the primary source of published trait data for this population came from and where the those data were collected. Formatted as first and last initial of the author of the publication or dataset and then the state the trait data comes from, ex) DB_WY = Dana Blumenthal's publication in list of data sources (below) and from a population in their data collected in WY. Data pulled from a global dataset available on TRY written as TRY_global. (*"NA" = not applicable). * "relation.to.EDGE.primary" = describes how close the trait data was collected to the focal population. Local = collected at or near EDGE site; Regional = collected in or average between values in same grassland type; Global = national or general averages global values if applicable. (*"NA" = not applicable). * "author_location.secondary" = if applicable, indicates the secondary source of published trait data for this population came from and where the those data were collected. (*"NA" = not applicable). * "relation.to.EDGE.secondary" = indicates where the secondary source of published trait data for this population came from and where the those data were collected. Formatted as first and last initial of the author of the publication or dataset and then the state the trait data comes from, ex) DB_WY = Dana Blumenthal's publication in list of data sources (below) and from a population in their data collected in WY. Data pulled from a global dataset available on TRY written as TRY_global. (*"NA" = not applicable). * "author_location.tertiary" = if applicable, indicates the last and minor source of published trait data for this population came from and where the those data were collected. (*"NA" = not applicable). * "relation.to.EDGE.tertiary" = indicates where the tertiary source of published trait data for this population came from and where the those data were collected. Formatted as first and last initial of the author of the publication or dataset and then the state the trait data comes from, ex) DB_WY = Dana Blumenthal's publication in list of data sources (below) and from a population in their data collected in WY. Data pulled from a global dataset available on TRY written as TRY_global. (*"NA" = not applicable). ## Sharing/Access information Original cover estimate data from two of the EDGE sites at the Sevilleta Wildlife Refuge in New Mexico are publicly available at the following location: * Trait data was derived from a mix of unpublished and open-access trait data associated with the following publications: * Stears, A. E., Adler, P. B., Blumenthal, D. M., Kray, J. A., Mueller, K. E., Ocheltree, T. W., Wilcox, K. R., &amp; Laughlin, D. C. (2022). Water availability dictates how plant traits predict demographic rates. *Ecology*, *103*(11). * Tucker, S. S. (2010). *Morphological and physiological traits as indicators of drought tolerence in tallgrass prarie plants*. Pittsburg State University * Laughlin, D. C., Leppert, J. J., Moore, M. M., &amp; Sieg, C. H. (2010). A multi-trait test of the leaf-height-seed plant strategy scheme with 133 species from a pine forest flora. *Functional Ecology*, *24*(3), 493–501. * Farrell, A. K. (2018). *Effects of Management on Functional Diversity in Restored Tallgrass Prairie Plant Communities*. Northern Illinois University * Craine, J. M., Nippert, J. B., Towne, E. G., Tucker, S., Kembel, S. W., Skibbe, A., &amp; McLauchlan, K. K. (2011). Functional consequences of climate change-induced plant species loss in a tallgrass prairie. *Oecologia*, *165*(4), 1109–1117. * Blumenthal, D. M., Mueller, K. E., Kray, J. A., Ocheltree, T. W., Augustine, D. J., &amp; Wilcox, K. R. (2020). Traits link drought resistance with herbivore defence and plant economics in semi‐arid grasslands: The central roles of phenology and leaf dry matter content. *Journal of Ecology*, *108*(6), 2336–2351. * TRY database: Kattge, J., Bönisch, G., Díaz, S., Lavorel, S., Prentice, L. C., &amp; Leadly, P. (2019). TRY plant trait database – enhanced coverage and open access. *Global Chnage Biology*, *26*(1), 119–188. ## Code/Software All analyses were conducted in R version 4.1.3 (R Core Team, 2022). R scripts used to complete the analysis in the associated publication are archived and available on Zenodo ([10.5281/zenodo.10198332](https://zenodo.org/doi/10.5281/zenodo.10198332)). In the folder named "code" in this repository, there are six .R scripts containing the code for all data manipulation, analyses, and figures included in the publication and supporting information. * "Data wrangling.R" script includes code to summarize data from larger EDGE dataset, calculate lambda, and create the **EDGE_covers.csv** and **all_pop_data.csv**. It is not necessary to run this script in order to replicate the analyses, but shows how data were compiled. * "summary stats.R" contains initial summary information about the different growth rates calculated and tests for differences in growth rate related to grassland type. * "responses analysis.R" contains the analysis of the relationships between growth rate in drought and growth rate with neighbors. * "traits analysis.R" contains the analysis of the relationship between traits and population growth in different precipitation conditions and neighbor abundances. * "figures.R" contains the code to reproduce all of the figures in the manuscript. * "supplemental info.R" contains the analyses and figures for information included in the supplemental.

# Access Points
https://datadryad.org/stash/dataset/doi:10.5061/dryad.1jwstqk1x