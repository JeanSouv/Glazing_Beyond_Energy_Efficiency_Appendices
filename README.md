# Glazing Beyond Energy Efficiency: Appendices

## Description

This repository gathers the codes and raw data used in the following doctoral thesis: Souviron, Jean. 2022. "Glazing Beyond Energy Efficiency: An Environmental Analysis of the Socio-Technical Trajectory of Architectural Glass." PhD diss., Université Libre de Bruxelles.

This repository is structured in three folders that correspond to the appendices in the three chapters of the thesis that use codes and extensive datasets:
- Appendix B relates to Chapter 2, "The Growing Environmental Impact of Architectural Glass."
- Appendix D relates to Chapter 4, "The Uncertainties of Efficiency."
- Appendix E relates to Section 6.1, "Flows of Architectural Glass Waste in Belgium, France and Europe."
- Appendix F relates to Section 6.2, "Urban Mining: Resources and Constraints."
- Appendix G relates to Section 6.4, "Glazing Stock Maintenance and the Time of Architecture."

The scripts in the three related folders (B, D and E) are also all available in PDF format so that they can be downloaded and read in any browser. To run the scripts and reproduce the results of the thesis, it is necessary to download the raw data. If you do not have access to the dissertation, the data or the codes, you can get them directly from me, please send a request to [jean.souviron@hotmail.fr](mailto:jean.souviron@hotmail.fr). Please get in touch if you find any mistake or problem in running these scripts and opening these files.

## Detailed Structure of the Repository

### Appendix_B:

The `B1_RawData` folder provides the data collected on the evolution of the flat glass industry, and more specifically the manufacturing of architectural flat glass since 1945 in the EU, France and Belgium. It contains three Excel files formatted to be used directly in the python script (Appendix B2). These Excel files are: `EU_RawData_VPython.xlsx`, `FR_RawData_VPython.xlsx`, and `BE_RawData_VPython.xlsx`.

`B2_FlatGlassIndustry_RetrospectiveMEFA.ipynb` is the Python script that post-processes the raw data according to the method explained in Section 2.1 of the thesis. This script also generates the graphs and tables.
`B2_FlatGlassIndustry_RetrospectiveMEFA.pdf` is a PDF version of the script.

### Appendix_D:

`D1_BEM_LCA_Hypotheses.xlsx` presents the main hypotheses of the building energy simulations (from building design to HVAC systems), with the list of scenarios.
`D2_lci` is a folder that gathers the life cycle inventory datasets resulting from the doctoral research and linked with the Biosphere 3 and Ecoinvent cut-off 3.7 database.
`D3_EnergyPlus` is a folder that gathers the EnergyPlus models in IDF format, together with weather data.
`D4_BEM.ipynb` is the Python script that conducts the building energy simulations. It relies on EnergyPlus. It exports in the outputs folder the results, which are then used to complete the life cycle inventory with energy flows during the use phase.
`D5_LCA.ipynb` is the Python script that conducts the life cycle impact assessment. It relies on Brightway2.

The two last scripts are available in PDF format: `D4_BEM.pdf` and `D5_LCA.pdf`.

Each of the two scripts generates the graphs and tables used in the PhD dissertation and can be run again to check the results.

### Appendix_E:

`E_FlowsOfIGUs_BE_FR.xlsx` presents the data collected from archives on the evolution of insulating glass unit consumption in France and Belgium since 1945. It shows the different calculation steps followed to estimate the evolution of the quantity of discarded glazing in relation to the date of their consumption and their lifespan. It also presents the graphs and table used in Section 6.1.

### Appendix_F:

`F_MFA_LaDefense_NorthDistrict.xlsx` presents the material and energy flow analysis related to the historical use of glazing in the business districts of La Défense and the Northern Quarter. This file gathers the dataset built according to archival research on the material history of the two districts. It then details the calculation steps followed to estimate the inflows, outflows and stocks. The estimation of the flows of energy, raw materials and CO2 relating to the manufacturing and recycling of the glazing stock is also detailed.

### Appendix_G:

`G_GrowthAndRecycling.xlsx` presents the data related to the historical evolution of the global and European flat glass consumption. It then models different recycling scenarios according to a series of future growth rates.
