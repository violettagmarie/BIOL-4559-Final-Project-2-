# BIOL-4559-Final-Project-2-
# Modeling Superspreading with Infection Trees and Group-Size Controls

This repository contains code and data for modeling superspreading in infectious disease outbreaks using infection trees and branching-process simulations. The analysis examines how imposing group-size controls—implemented as tail-cut thresholds on secondary infections—alters outbreak size and extinction dynamics across multiple real-world transmission networks.


## Repository Structure

.
├── code/
│ └── modeling_superspreading.ipynb
├── dataset/
│ ├── edgelists1.csv
│ └── node_info1.csv
└── README.md

Copy code



### `code/`
The `modeling_superspreading.ipynb` notebook contains the full analysis workflow:
- Construction of infection trees from empirical transmission edge lists.
- Estimation of Negative Binomial offspring distributions using the method of moments.
- Simulation of Galton–Watson branching processes with and without group-size controls.
- Sensitivity analysis over a range of tail-cut thresholds to quantify cases averted.
- Visualization of outbreak-specific and aggregate intervention effects.


### `dataset/`
The `dataset/` directory includes the raw data used in the simulations:
- `edgelists1.csv`: Directed transmission edge lists for multiple outbreaks, identified by disease ID.
- `node_info1.csv`: Node metadata defining the population at risk for each outbreak.


## Requirements

The analysis requires Python 3 and the following packages:
- pandas
- numpy
- networkx
- matplotlib
- scipy


