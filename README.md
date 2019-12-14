# forked for WERA systems
requires additional library matWERA  
to install all required libraries  
git clone https://github.com/gvoulgaris0/matWERA  
git clone https://github.com/g2e/m_map  
git clone https://github.com/rowg/hfrprogs  

and the program  
git clone https://github.com/dougcahl/lera_DPd  
git clone https://github.com/dougcahl/lera_DP_testdata_wera  

Then edit HFR_DP_master_LERA_gtn.m to add the full paths before running.     
The example data in lera_DP_testdata_wera includes necessary scripts for antenna pattern calculations. 

The processing scripts for raw WERA data (from .RAW and .SORT) are available in the WERA_to_DP repo that make a compatible .mat file for the forked lera_DPd repo here. This fork will automatically process either of these (from .RAW or .SORT) created by WERA_to_DP.   
git clone https://github.com/dougcahl/WERA_to_DP  
git clone https://github.com/dougcahl/wera_raw_data  

Dec. 2019 -- Douglas Cahl, dcahl@geol.sc.edu



# lera_DPd

This package is the Public version of the HFR_DP software for processing LERA-type HF radar data sets.

This package contains the master programs to process LERA-type HF Radar system data in Matlab from the decimated time series data (a *.mat file pre-divided into chirps) to radial velocities averaged over an azimuthal window for a particular radar site.  This code allows for the use of MKII or MKIII radar systems and direction finding methods including; MUSIC, MLE, and WSF. 

See HFR_DP_LERA_SETUP_README.m for setup and package details.

See:

Kirincich, A., B. Emery, L. Washburn, and P. Flament, 2018. Surface Current Mapping Using a Hybrid Direction Finding Approach for Flexible Antenna Arrays, JOAT (submitted). 

for details about the radar systems, the processing methodologies, and validation comparisons.

This package is citable as DOI:10.5281/zenodo.3353662 .

Anthony Kirincich 
WHOI-PO 
akirincich@whoi.edu
