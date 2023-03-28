# Preprocessing Framework for Cleaning MR Images
This repository contains a preprocessing framework for cleaning MR images based on denoising filters. The aim of this project is to decide the correct order of preprocessing filters as well as their types. The denoising filter used in this project is expected to preserve edges while removing noise.

## Data
This project uses simulated MRI volumes of T1, PD, and T2 modality data set (1mm, 0% of noise, and intensity non-uniformity of 0%) from BrainWeb as clean images. The unclean images are downloaded from BrainWeb images of T1, PD, and T2 data set (1mm, 3% and 9% of noise, and intensity non-uniformity of 0%).

## Preprocessing T1, PD, and T2 Images
To preprocess the unclean images, denoising filters are applied in the correct consecutive order. The processed image is then compared with respect to the clean image by the Coefficient of Variation (CV) metric, which is a popular measure of intensity variation for a given tissue class (C), defined as the standard deviation σ divided by the mean value µ:

CV (C) = σ(C)/µ(C)

The higher the CV, the greater the dispersion in the variable.

The quantitative comparison results are presented in a neat-table, and the image data, including clean and unclean images as well as processed images, is visualized.

## Conclusion
This project presents a preprocessing framework for cleaning MR images based on denoising filters. The denoising filter used in this project preserves edges while removing noise. The quantitative comparison of the processed images with the clean images using the Coefficient of Variation (CV) metric suggests that the processed images have lower dispersion in the variable.
