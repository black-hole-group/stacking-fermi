# Fermi-LAT Stacking Analysis 

Useful methods and functions to perform stacking analysis of Fermi-LAT gamma-ray data. The current version was made for Fermitools 2.0.8 and Fermipy 1.0.0.

`tracing_TS.py`  
Pipeline for implementing a basic analysis on a list of targets. Includes options to trace TS (Test Statistic) profiles for stacking and generating mock data for statistical analysis.

`Stack_dwarfs.ipynb`  
 Jupyter notebook with example implementation of the `trace_profile()` algorithm for a sample of  dwarf galaxies with evidence for AGN. 

`fermi_utils.py`  
 Miscellaneous utilities for working with Fermipy and Fermi-LAT data analysis, including:
 - Parameter extraction functions (pars)
 - File reading utilities (get_pars)
 - Date/time conversion functions (date_day, fermi_time)
 - Mock source generation (gen_rd_pos)
 - ROI indexing functions (roi_i)
 - Text file parsing utilities (open_txt)
 - Distance calculations (dist, Dist)
 - Statistical functions (gauss, chance)

`Basic_calc_num.py`  
 A few mathematical tools for numerical computation.