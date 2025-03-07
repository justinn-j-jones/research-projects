# Using aerial and terrestrial mobile lidar with high-resolution imagery to estimate biophysical parameters of urban trees
Urban Forestry & Urban Greening

This directory contains all python and R notebooks used to process and analyze data for our projects. Some files, such as CHM.tif and MLS.las are much too large to upload here, but a sample of 10 trees is provided in the Sample sub-directory. Output shapefiles, CSVs, etc. can be found in the corresponding Output folders. 

## Sample mobile lidar scan (MLS) LAS
Sample of 10 trees scanned with MLS from our project. The complete scans are far too large to upload here. 

## Appendix A: 00_LAS_synpts_raster
This notebook assumes the ipynb resides directly in the “main directory” with a ‘_input’ folder housing the input files. We will create and use an ‘output’ folder for output files.

"Synthetic Points from Raster $(SPR)$" will take an input raster and create a single point from each cell with the cell value, and output a new TXT, which can then be read into software (such as Quick Terrain Modeler) as XYZ (ASCII) and exported as LAZ / LAS. 
<br><br>
This is useful for gap-filling from a DEM or generating a "top of canopy LAS" from a CHM.
<br><br>
If it is necessary to replace negative Z values with 0, the last cell will write a new TXT. 

## Appendix B: 01_RMD1
This R markdown notebook is the first step towards automating the process of measuring trees.

This notebook assumes the RMD resides directly in the "main directory" with a '\_input' folder housing the input files. We will create and use an 'output' folder for output files.

## Appendix C: 02_lidR_tt_cw
This ipynb is the second step towards automating the process of measuring trees.

This notebook assumes the ipynb resides directly in the “main directory” with a ‘_input’ folder housing the input files. We will create and use an ‘output’ folder for output files.

- This notebook will take the `lidR` output tt points and cw polygons as inputs. 
- These inputs will be joined to field data points and calculate Improved Crown Width (ICW). 
- Output will be a CSV file and histograms. 

## Appendix D: 03_RMD2
This R markdown notebook is the third step towards automating the process of measuring trees.

This notebook assumes the RMD resides directly in the "main directory" with a '\_input' folder housing the input files. We will create and use an 'output' folder for output files.

## Appendix E: 04_TreeLS_inv
This ipynb is the fourth step towards automating the process of measuring trees.

This notebook assumes the ipynb resides directly in the “main directory” with a ‘_input’ folder housing the input files. We will create and use an ‘output’ folder for output files.

- This notebook will take the `TreeLS` output CSV as an input and join to existing inventory list to create one master inventory. 
- After joining, subsets will be created to run stats. 
- Outputs will be CSV and SHP of master inventory list along with scatterplots. 

# Contact 

**Justinn J. Jones ’24, GISP**

Graduate Research Assistant / FAA sUAS RP

LASERS Lab / WFES 360

Department of Ecology & Conservation Biology

College of Agriculture & Life Sciences

justinn.j.jones@tamu.edu

**TEXAS A&M UNIVERSITY**