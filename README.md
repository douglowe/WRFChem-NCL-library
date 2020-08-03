# WRFChem-NCL-Library

A library of WRF-Chem focused NCL functions for use in other 
data extraction / plotting scripts.

To use these, add them to your github repository using:
git submodule add https://github.com/douglowe/WRFChem-NCL-library.git library

You will then need to set the `WRF_NCL_ROOT` environmental variable, e.g.:
```
export WRF_NCL_ROOT=[path to repository directory]
```

This is because the `variable_loading_library.ncl` library uses this variable to
find the `WRFCHEM_misc_stats.ncl` library:
```
load "$WRF_NCL_ROOT/library/WRFCHEM_misc_stats.ncl"
```