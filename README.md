# Real-Time MRI Cardiac Function Analysis in Pediatric CHD Patients

**Status:** This paper is currently under revision.

## Overview

This repository contains the code used in the paper titled "First Experiences with Real-Time MRI-Based Investigation of Respiratory Influence on Cardiac Function in Pediatric Congenital Heart Disease Patients with Chronic Right Ventricular Volume Overload".

The code is provided as a Jupyter notebook and is designed to analyze cardiac function in pediatric CHD patients with chronic RV volume overload using real-time magnetic resonance imaging (RT-MRI) during free breathing (FB).

## Binning Process

- RT magnetic resonance images were binned based on respiration and ECG-derived RR intervals.
- Respiration information was derived from signal intensity (SI) changes related to diaphragmatic movement in regions of interest (ROIs).
- Further RT-data processing was done in Python, adapting published open-source packages such as Numpy and pydicom.
- The moving median based on the previous and subsequent 10 SI values was used to provide information on the respiratory phase.
- RT-images were binned in eight respiratory classes and 25 cardiac phases.
- In case of overfilled bins, images were filtered using an efficient state-of-the-art subpixel phase correlation analysis.

For a detailed description of the binning process and other methodologies, please refer to the paper.

## Sample Data

Sample data can be requested from:
- Prof. Dr. Pillekamp (pillekamp@uni-duesseldorf.de)
- Dr. Röwer (Lena.Roewer@med.uni-duesseldorf.det)

## Dependencies

- Python (v3.8.4)
- Numpy
- pydicom
- [Additional dependencies as per the Jupyter notebook]

## Usage

1. Clone the repository.
2. Install the required dependencies.
3. Open the Jupyter notebook and follow the instructions provided within.
