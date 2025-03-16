# ThermalHR: Heart Rate Estimation from Thermal Videos

This repository contains code for estimating heart rate from thermal camera recordings. The process consists of the following steps:

- Video Processing:
  The code reads thermal video recordings captured using a FLIR camera.
  It converts .seq format videos into individual 16-bit TIFF frames.

- Region of Interest (ROI) Detection:
  Each frame is analyzed to detect and extract the Region of Interest (ROI).

- Temperature Signal Extraction:
  The average temperature values within the ROI are computed for each frame.

- Signal Processing:
  The extracted signal undergoes filtering and normalization.
- Principal Component Analysis (PCA) and Independent Component Analysis (ICA) are applied to enhance the signal.

- Frequency Analysis:
  A Fast Fourier Transform (FFT) is performed to identify the dominant frequency, which corresponds to the estimated heart rate.
