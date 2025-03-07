# Using aerial and terrestrial mobile lidar with high-resolution imagery to estimate biophysical parameters of urban trees
Urban Forestry & Urban Greening

## Appendix A: A__LAS_synpts_raster.ipynb
This notebook assumes the ipynb resides directly in the “main directory” with a ‘_input’ folder housing the input files. We will create and use an ‘output’ folder for output files.

"Synthetic Points from Raster $(SPR)$" will take an input raster and create a single point from each cell with the cell value, and output a new TXT, which can then be read into software (such as Quick Terrain Modeler) as XYZ (ASCII) and exported as LAZ / LAS. 
<br><br>
This is useful for gap-filling from a DEM or generating a "top of canopy LAS" from a CHM.
<br><br>
If it is necessary to replace negative Z values with 0, the last cell will write a new TXT. 

## Appendix B: B__RMD1.Rmd
This R markdown notebook is the first step towards automating the process of measuring trees.

This notebook assumes the RMD resides directly in the "main directory" with a '\_input' folder housing the input files. We will create and use an 'output' folder for output files.

## Appendix C: C__tt_cw_v2.ipynb
This ipynb is the second step towards automating the process of measuring trees.

This notebook assumes the ipynb resides directly in the “main directory” with a ‘_input’ folder housing the input files. We will create and use an ‘output’ folder for output files.

- This notebook will take the `lidR` output tt points and cw polygons as inputs. 
- These inputs will be joined to field data points and calculate Improved Crown Width (ICW). 
- Output will be a CSV file and histograms. 

## Appendix D: D__RMD2.Rmd
This R markdown notebook is the third step towards automating the process of measuring trees.

This notebook assumes the RMD resides directly in the "main directory" with a '\_input' folder housing the input files. We will create and use an 'output' folder for output files.

## Appendix E: E__TreeLS_inv_v2.ipynb
This ipynb is the fourth step towards automating the process of measuring trees.

This notebook assumes the ipynb resides directly in the “main directory” with a ‘_input’ folder housing the input files. We will create and use an ‘output’ folder for output files.

- This notebook will take the `TreeLS` output CSV as an input and join to existing inventory list to create one master inventory. 
- After joining, subsets will be created to run stats. 
- Outputs will be CSV and SHP of master inventory list along with scatterplots. 
