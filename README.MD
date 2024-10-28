# Background Subtraction for Light Curves

This repository contains code for performing background subtraction on light curves using data from FITS files. The main script is implemented in a Jupyter Notebook (Bag_sub.ipynb).

## Repository Structure
.DS_Store
Bag_sub.ipynb
Datasets/
    glg_tte_n1_bn111220486_v00.fit
    glg_tte_n1_bn141031998_v00.fit
    glg_tte_n5_bn170817529_v00.fit
    glg_tte_n6_bn090510016_v00.fit
    glg_tte_n6_bn200907957_v00.fit
    glg_tte_n6_bn230428381_v00.fit
    glg_tte_n8_bn090719063_v00.fit

## Requirements

- Python 3.9
- Jupyter Notebook
- NumPy
- Matplotlib
- SciPy
- Astropy

You can install the required packages using pip: `pip install numpy matplotlib scipy astropy jupyter`

## Usage
1. **Load FITS Data**: The function load_fits_data in the notebook loads the time data from a specified FITS file.

2. **Create Histogram**: Generate a histogram of the time data to get counts.

3. **Define Background Region**s: Define the regions for background data.

4. **Select Background Data**: Use the select_background function to select background data.

5. **Fit Polynomial to Background**: Fit a polynomial to the background data.

6. **Subtract Background**: Subtract the background model from the original histogram.

7. **Plot Results**: Plot the original histogram, background model, and background-subtracted data.

## Acknowledgements
This project uses data from the Fermi Gamma-ray Space Telescope.