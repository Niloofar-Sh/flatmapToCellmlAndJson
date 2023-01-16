# flatmapToCellmlAndJson
A Jupyter Notebook to generate a CellML file for the selected structures in the Generic Cell Flatmap

👉 To use the code, you need to download and save the required ontologies as .csv files. 👈

- OPB: https://bioportal.bioontology.org/ontologies/OPB

- GO: https://bioportal.bioontology.org/ontologies/GO

- FMA: https://bioportal.bioontology.org/ontologies/FMA

- CHEBI: https://bioportal.bioontology.org/ontologies/CHEBI

Since the size of the stored ontologies exceeds the GitHub upload limit, the ontologies' .csv files are not uploaded here. Change the address which points to the ontologies on your local machine.


The Jupyter Notebook **CellmlScriptProductionEnzymes_findValueRange.ipynb** is the main code file.

The enzymes file includes the .cellml files which describe the parameters of the structures found on the Generic Cell Flatmap.

The **GFG.cellml** & **GFG.txt** are the files which include the bond graph composed model of the selected structures on the Generic Cell Flatmap.

The **units_BG.cellml** is the file for units which will be imported to GFG.cellml.

The **jsonForCellml.json** is a JSON file which gives further information on the generated cellml file (here, GFG.cellml). It includes the variable names used in the CellML file, their RDFs, RDF meanings, values, and units.

To understand the range of values that others have used for the same biochemical parameters in their models on PMR, we search for all the annotations on those models and extract the values assigned to them. Here, instead of an online search on PMR, we have stored some exemplar annotated CellML models in **Exemplar models on PMR**. This will be later extended to an online search.
