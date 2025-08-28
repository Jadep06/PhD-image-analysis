As part of my PhD project I was trying to quantify the mechanical properties of cells of the intestinal epithelium during damage induced regeneration and tumorigenesis.
A large part of this work is online ahead of print https://www.biorxiv.org/content/10.1101/2025.04.16.649133v1.full

To quantify the mechanical properties of cells is difficult in this system as it is a complex multilayer tissue- with ECM and visceral muscle surrounding the enterocytes, approaches
like AFM do not give us a good readout of mechanics specifically in the epithelial cell compartment. Therefore using imaging and computational image analysis, we looked at changes in 
cell morphology as a readout of changes in cell mechanical state as there is a significant body of literature which shows that cell shape changes directly show a mechanical change in a cell.

Originally I was using a programme in MATLAB called deproj (https://bmcbiol.biomedcentral.com/articles/10.1186/s12915-021-01037-w) to perform an analysis of cell morphology including 
eccentricity- however, this required a large amount of preprocessing by hand. As it is in MATLAB it was also not able to be used by members of my research group who do not have access 
to a MATLAB liscence. Therefore I wrote a python script to perform the same analysis (eccentricity from membrane stain 1.ipynb) and have also written a batch file for analysis of folders
of images (batch eccentricity processing from membrane stain.ipynb). Using this I was also able to calculate other properties which are indicative of cell forces such as fluidity like
cell shape index.

I also used another programme written in MATLAB which uses Bayesian Force Inference to infer tension and pressure in cells (https://www.nature.com/articles/s41598-019-50690-3).

I have also written another image analysis programme in python to analyse RNAscope dual colour data. I segmented cells and selected nuclei positive for CD31 to select endothelial cells and then 
measured the amount of Piezo1 RNA detected in these cells (rnascope analysis.ipynb).

