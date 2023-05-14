# Distribution of Relaxation Times based on Lasso regression
Here we present a novel approach for the analysis of IMPS data, based on the calculation of the DRT curve using Lasso regression. The algorithm is written in Python. We suggest the use of Google Colab for running the code.
# How to use it
Copy and paste the code "GL-DRT.ipynb" in Google Colab editor. In the "content" folder, upload a file made by three columns: frequency (Hz), real part (A/W) and imaginary part (A/W) of the IMPS spectrum. If there are header lines at the beginning of the file you can skip them by changing skiprows number.
In the function "cvxpy_solve_qp()" you can modify the last parameter, which represents the regularization parameter, according to the result of the fit.
# Description of the algorithm
A detailed description of the algorithm is reported here: https://pubs.acs.org/doi/full/10.1021/acs.jpcc.3c00770
# Example
In the folder "Hematite data" there is a set of IMPS spectra recorded at different potentials applied to the PEC cell (these raw data are the same used in the reference article, without any normalization). If you copy and paste them in the "content" folder you can run the the code "multi_file_GL-DRT.ipynb" to get the L-DRT for any file. In this case the algorithm is included in a for loop and repeats the analysis for every file in the folder.
The output graphs represent the IMPS data with the fit (first), the descrete L-DRT curve (second), the GL-DRT curve (third), J_photo, J_Gartner and J_rec (fourth) and k_rec and k_tr (fifth).
# Support
If you need support write to: alberto.piccioni@unibo.it, pierpaolo.vecchi2@unibo.it or raffaello.mazzaro@unibo.it
# To cite this work
Piccioni, A.; Vecchi, P.; Vecchi, L.; Grandi, S.; Caramori, S.; Mazzaro, R.; Pasquini, L. Distribution of Relaxation Times Based on Lasso Regression: A Tool for High-Resolution Analysis of IMPS Data in Photoelectrochemical Systems. J. Phys. Chem. C 2023.

https://pubs.acs.org/doi/10.1021/acs.jpcc.3c00770
