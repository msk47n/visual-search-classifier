# visual-search-classifier

## Overview

This project implements and compares three machine learning models (MLP, SVM, and CNN) to classify visual search images based on target presence. The goal is to evaluate the performance of different model architectures on the same dataset.

## Example Input / Output

### Example 1

Input:
![Example input](examples/stimulus_ss_4.png)

Output:
Predicted class: Target present 

### Example 2

Input:
![Example input](examples/stimulus_ss_8.png)

Output:
Predicted class: Target absent

### Results

MLP:
![Result_1](results/mlp_result.png)

Shaded region represents 95% confidence intervals. The plot shows accuracy over different features tested for an MLP model.

SVM:
![Result_2](results/SVM_result.png)

The bright yellow colour represents high accuracy. The plot shows accuracy with varying c and gamma parameters of an SVM model.

CNN:
![Result_3](results/CNN_result.png)

Shaded region represents 95% confidence intervals. The plot shows accuracy over different kernel sizes tested for a CNN model.


## Results Summary

The CNN achieved the highest classification accuracy, followed by the SVM, while the MLP had the lowest accuracy.

One likely reason for CNN's superior performance is its ability to process images in their original spatial structure. Unlike MLP and SVM, which operate on flattened image vectors, CNNs preserve spatial relationships between pixels. This allows CNNs to learn meaningful spatial features relevant to visual search tasks.

The SVM outperformed the MLP, likely due to its use of a non-linear decision boundary, which enables it to better separate complex patterns and maintain robustness to noise in high-dimensional input space.


## Notes

This project was developed as part of a course project. The code reflects the experimental workflow used during development.

## Author

Saad Khan

