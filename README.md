# pyROWSTACK
This is a Jupyter notebook to stack multiple rows of a detector (8K x 2K) after bias and dark corrections. It presents an enhancement of the dynamical range of a CMOS detector.

#  Background

CMOS detectors can be used to reach arbitrarily high signal-to-noise ratio as it is possible to read different parts (row-wise readout scheme) of the detector at different rates. An optical setup was made to form Newton's ring. Two transmitted Airy disk patterns were projected onto the CMOS detector. The centre of brightest pattern was located and the corresponding row was read out several times. Similarly, the centre of the faintest pattern was identified and the row was considered for one read out.

**Jupyter Notebook Author:** Supriyo Ghosh

## Objective
Process a raw image (object image), stack the brightest row and create a plot for bightest and faintest rows of the Airy  disks.

## Key steps
First step:

- Read the object image and plot it
- Separate out the bright chunk and faint row
- Based on the repetation number of the bright row, seperate out bright row from the bright chunk and stack the rows along an axis
- Add all bright rows
- Create a plot of bright row and the faint row

Second step:

- The object image is corrected for bias (For that, master bias is created by median combination).
- Repate the First step

Thrid step:

- The image is corrected for bias (created in the Second step) and dark (master dark is created by median combination).
- Repate the First step


### Python modules
* python 3
* numpy
* astropy
* matplotlib

For any queries, suggestions and comments, please do not hesitate to contact me at supriyoani89@gmail.com. Many thanks.
