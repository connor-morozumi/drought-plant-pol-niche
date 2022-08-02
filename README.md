# drought-plant-pol-niche

This is the code repository for the published paper: Simultaneous niche expansion and contraction in plant-pollinator networks under drought

Authors: Connor Morozumi, Loy Xingwen, Victoria Reynolds, Annie Schiffer, Beth Morrison, Jade Savage, Berry Brosi

DOI: 10.1111/oik.09265

# Scope
How flexible are interaction niches under altered abiotic conditions? Here we investigate how plant-pollinator interaction networks respond to drought. 

This repository contains all code for Morozumi et al. 2022 manuscript investigating the effects of drought on plant-pollinator niche breadth. We utilized visitation data from three sites over five years, 2016-2020 with 2018 and 2020 determined to be drought years. We wanted to understand whether interactions in drought were getting more general (niche broadening) when floral resources were depressed. Additionally, we  want to know whether this niche broadening is associated with changes in interaction abundances and/or species turnover between the drought and non-drought years. To do this we devised a null model (bootstrap type procedure) and calculated a series of network summary metrics on the 1000 bootstrapped replicates. We used permutation based statistical comparison of network metric values to the raw value calculated in drought year. Additionally we partitioned the data by site and year to understand the contributions of these factors to the overall findings. Finally, we analyzed weather data to confirm drought year determination.

# Data
This repository contains three datasets

+ total visits per site per year by each pollinator taxa: `visitation.csv`
+ floral abundance: `floral.abundance.csv`
+ weather data from the Gothic field station: `gothicweather.csv`

# Code Overview
We've combined all analyses for the paper into one R Notebook titled `Drought.web.Rmd`. This consists of:



1. Null model bootstrap
+ Abundance-based
+ Controlling for species turnover
+ By site and year
3. Floral Abundance
4. Drought Analysis
+ NMDS
+ PERMANOVA

