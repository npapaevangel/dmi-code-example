# dmi-code-example
# DMI Code Example — NWP Convective Storm Masking & Ensemble Post-processing

This repository contains a small code example used for technical discussion.

The notebook demonstrates a typical post-processing workflow on NWP ensemble output:

- loading CTRL and SEED ensemble members,
- computing maximum vertical velocity over altitude,
- defining a convective storm mask using physical thresholds,
- expanding the mask to include neighboring grid points,
- applying the mask to a microphysical variable (TQI),
- computing domain-mean time series per ensemble member,
- exporting results to NetCDF.

## Files
- `Example_code_DMI_Nikos_Papaevangelou.ipynb` — main Jupyter notebook with the full workflow.

## Data
Model output data (NetCDF files) are not included.

The data path can be set at the top of the notebook:
```python
directory_path = "/path/to/case_folder/"
