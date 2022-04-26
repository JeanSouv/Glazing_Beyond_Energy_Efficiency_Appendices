# Glazing Beyond Energy Efficiency: Appendices

## Description

This repository gathers the codes and raw data used in the following doctoral thesis: Souviron, Jean. 2022. "Glazing Beyond Energy Efficiency: An Environmental Analysis of the Socio-Technical Trajectory of Architectural Glass." PhD diss., Université Libre de Bruxelles.

This repository is structured in three folders that correspond to the appendices in the three chapters of the thesis that use codes and extensive datasets:
- Appendix B corresponds to Chapter 2, "The Growing Environmental Impact of Architectural Glass;"
- Appendix D corresponds to Chapter 4, "The Uncertainties of Efficiency;"
- Appendix E and corresponds to Chapter 6, "Challenges in Maintaining the Glazing Stock."


The scripts in the three related folders (B, D and E) are also all available in PDF format so that they can be downloaded and read in any browser. To run the scripts and reproduce the results of the thesis, it is necessary to download the raw data. If you do not have access to the dissertation, the data or the codes, you can get them directly from me, please send a request to [jean.souviron@hotmail.fr](mailto:jean.souviron@hotmail.fr).

## Detailed Structure of the Repository

### Folder B:

The `B1_RawData` folder provides the data collected on the evolution of the flat glass industry, and more specifically the architectural flat glass production in the EU, France and Belgium. It contains three Excel files formatted to be used directly in the python script and which are: `EU_RawData_VPython.xlsx`, `FR_RawData_VPython.xlsx`, and `BE_RawData_VPython.xlsx`.

`B2_FlatGlassIndustry_RetrospectiveMEFA.ipynb` is the Python script that post-processes the raw data according to the method explained in Section 2.1 of the thesis. This script also generates the graphs and tables.
`B2_FlatGlassIndustry_RetrospectiveMEFA.pdf` is a PDF version of the script.

### Folder D:

`D1_BEM_LCA_Hypotheses.xlsx` presents the main hypotheses of the building energy simulations (from building design to HVAC systems), with the list of scenarios.
`D2_lci` is a folder that gathers the life cycle inventory datasets resulting from the doctoral research and linked with the Biosphere 3 and Ecoinvent cut-off 3.7 database.
`D3_EnergyPlus` is a folder that gathers the EnergyPlus models in IDF format, together with weather data.
`D4_BEM.ipynb` is the Python script that conducts the building energy simulations. It relies on EnergyPlus. It exports in the outputs folder the results, which are then used to complete the life cycle inventory with energy flows during the use phase.
`D5_LCA.ipynb` is the Python script that conducts the life cycle impact assessment. It relies on Brightway2.

The two last scripts are available in PDF format.

Each of the two scripts generates the graphs and tables used in the PhD dissertation and can be run again to check the results.

### Folder E:

Please get in touch if you find any mistake or problem in running these scripts.