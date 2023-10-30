# Real-Time MRI Cardiac Function Analysis in Pediatric CHD Patients

## Overview

This repository hosts the code and methodology associated with the research paper: 

**"First Experience with Real-Time Magnetic Resonance Imaging-Based Investigation of Respiratory Influence on Cardiac Function in Pediatric Congenital Heart Disease Patients with Chronic Right Ventricular Volume Overload."** 

Röwer, L.M., Radke, K.L., Hußmann, J., Malik, H., Eichinger, M., Voit, D., Wielpütz, M.O., Frahm, J., Klee, D., & Pillekamp, F. (2023). *Pediatr Radiol*. [DOI: 10.1007/s00247-023-05765-9](https://doi.org/10.1007/s00247-023-05765-9).

This study employed real-time magnetic resonance imaging (RT-MRI) to analyze cardiac function in pediatric CHD patients with chronic RV volume overload during free breathing (FB).

## Binning Process

- RT magnetic resonance images were categorized based on respiration and ECG-derived RR intervals.
- Respiration data was inferred from signal intensity (SI) fluctuations associated with diaphragmatic motion in specific regions of interest (ROIs).
- Subsequent RT-data processing was conducted in Python, leveraging widely-recognized open-source libraries such as Numpy and pydicom.
- A moving median, considering the 10 preceding and 10 subsequent SI values, was employed to discern the respiratory phase.
- RT-images were categorized into eight respiratory classes and 25 cardiac phases.
- If bins were overpopulated, images underwent filtration using a cutting-edge subpixel phase correlation analysis.

For an in-depth exploration of the binning process and other methodologies, kindly refer to our [published paper](https://doi.org/10.1007/s00247-023-05765-9).

## Sample Data

For a sample dataset, please reach out to:
- Prof. Dr. Pillekamp: [pillekamp@uni-duesseldorf.de](mailto:pillekamp@uni-duesseldorf.de)
- Dr. Röwer: [Lena.Roewer@med.uni-duesseldorf.de](mailto:Lena.Roewer@med.uni-duesseldorf.det)

## Dependencies

- Python (v3.8.4)
- Numpy
- pydicom
- [Further dependencies as detailed in the Jupyter notebook]

## Usage

1. Clone or download the repository.
2. Install the necessary dependencies.
3. Launch the Jupyter notebook and adhere to the instructions embedded within.

---

**Citation**: If you find this work beneficial or utilize it in your research, please cite our paper:

```
@article{rower2023realtime,
  title={First Experience with Real-Time Magnetic Resonance Imaging-Based Investigation of Respiratory Influence on Cardiac Function in Pediatric Congenital Heart Disease Patients with Chronic Right Ventricular Volume Overload},
  author={Röwer, Lena Maria and Radke, Karl Ludger and Hußmann, Janina and Malik, Halima and Eichinger, Monika and Voit, Dirk and Wielpütz, Mark Oliver and Frahm, Jens and Klee, Dirk and Pillekamp, Frank},
  journal={Pediatr Radiol},
  year={2023},
  doi={10.1007/s00247-023-05765-9}
}
```
