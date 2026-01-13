# Supernovae 3D Visualization and Parameter Fitting

This repository contains code and interactive visualizations based on the Pantheon+SH0ES Type Ia supernova sample.

---

## Files

### `sne_pipeline.ipynb`

This Jupyter notebook runs the full data-processing and fitting pipeline. It:
- loads the Pantheon+SH0ES supernova data,
- computes comoving, luminosity, and angular-diameter distances,
- constructs 3D Cartesian coordinates in both equatorial (ICRS) and Galactic frames,
- performs a generalized least-squares fit for distance-ladder parameters using the full STAT+SYS covariance.

The cosmology used to compute distances is for visualization purposes only and does not affect the parameter-fitting results.

---

### Interactive 3D Visualizations (`.html`)

The two `.html` files are standalone interactive Plotly visualizations.

To view an interactive plot, download the `.html` file and open it locally in a web browser.

#### `pantheon_3d_distribution_CMBdipole.html`

Shows the full supernova sample (calibrators and Hubble-flow SNe) in 3D, together with the CMB dipole axes.

#### `pantheon_3d_distribution_Calibrators_HF.html`

Displays calibrator and Hubble-flow supernovae separately in both equatorial and Galactic coordinate systems.  
Use the dropdown menu in the top-left corner to switch between coordinate frames and subsets.

---

## Data

All supernova data and covariance matrices are from the Pantheon+SH0ES Data Release:  
https://github.com/PantheonPlusSH0ES/DataRelease
