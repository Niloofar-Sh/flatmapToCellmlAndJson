# flatmapToCellmlAndJson
A Jupyter Notebook to generate a CellML file for the selected structures in the Generic Cell Flatmap

The description for each cell of the Jupyter Notebook is provided in order as follows:

**Cell 1:** The required libraries

**Cell 2:** To use the code you need to download and save the required ontologies as .csv files. 

OPB: https://bioportal.bioontology.org/ontologies/OPB

GO: https://bioportal.bioontology.org/ontologies/GO

FMA: https://bioportal.bioontology.org/ontologies/FMA

CHEBI: https://bioportal.bioontology.org/ontologies/CHEBI

Since the size of the stored ontologies exceeds the GitHub upload limit, the ontologies' .csv files are not uploaded here.
Change the address which points to the ontologies on your local machine.

**Cell 3:** Here, a dictionary (templateGroups) has been generated to define which group of transporters/structures belong to which template. Template names are the keys M1, M2, ... and the dictionary values represent the name of the structures belonging each template. For each transporters/structure we need to have a CellML file in which their specific parameters are initialized and annotated. These files don't need to include any mathematical equations.

**Cell 4:** Here, we assume that the structures SLC1 & SLC2 are selected from the flatmap. The goal is to generate a bond graph model of the composed structure (SLC1+SLC2) and provide a CellML file along with a JSON file. In this cell we find the required template to use for the structure names. The dictionary 'inUse' maps between the selected structures and their templates.

**Cell 5:** 

