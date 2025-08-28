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
<img width="1156" height="461" alt="Screenshot 2025-08-28 4 08 34 PM" src="https://github.com/user-attachments/assets/646e1b5f-f8de-4af1-be80-872381b2a1ea" />
<img width="1198" height="374" alt="Screenshot 2025-08-28 4 07 46 PM" src="https://github.com/user-attachments/assets/734a4af7-c286-4def-b781-254d2251edb0" />


I also used another programme written in MATLAB which uses Bayesian Force Inference to infer tension and pressure in cells (https://www.nature.com/articles/s41598-019-50690-3).


<img width="482" height="292" alt="Screenshot 2025-08-28 4 09 16 PM" src="https://github.com/user-attachments/assets/c10d284e-e139-44f5-8663-ce5c6e4531e3" />

I have also written another image analysis programme in python to analyse RNAscope dual colour data. I segmented cells and selected nuclei positive for CD31 to select endothelial cells and then 
measured the amount of Piezo1 RNA detected in these cells (rnascope analysis.ipynb).

<img width="1172" height="451" alt="Screenshot 2025-08-28 4 13 17 PM" src="https://github.com/user-attachments/assets/a229132f-07aa-46fc-9348-0fe3a5f680af" />




