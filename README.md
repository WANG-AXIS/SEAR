# SEAR
This repository includes the data and final results presented in the manuscript Data for "A Feasibility Analysis on Simultaneous Electron Density and Attenuation Coefficient Reconstruction" A directory exists for each experiment conducted:

-regular: Original, generated 2D Shepp-Logan phantoms.

-oos: Out-of-sample (more internal ellipses) generated 2D Shepp-Logan phantoms (test sets only).

-medical: Simulated abdominal images from a human CT scan.

-tumor: Simulated abdominal images from a human CT scan with or without an added lesion.

-eres: Generatd 2D Shepp-Logan phantoms, simulated with finite energy resolution.

Each contains two subdirectories: 'ground_truth': contains ground truth simulated images. 'reconstruction': contains reconstruction results from the final iteration of the reconstruction algorithm.

Two types of images are contained in each file:

-Simulated electron density images (denoted as 'alpha').

-Simulated monochromatic attenuation (80keV) images (denoted as 'mu'), which were used for the attenuation reconstruction target..

For reconstruction results, 'alpha' image files contain 5 different reconstruction estimations based on different detected scatter energies (see manuscript for details). All simulated images are stored as .mat files.

Note: medical/reconstruction/mu_train is split into two files to decrease maximum file size.
