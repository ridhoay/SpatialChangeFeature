# SpatialChangeFeature

A Spatial Change Feature-Based Deep Learning Method for Multi-Mineral Segmentation in Micro-CT Rock Images
## Thesis Project
This repository contains the implementation for the research titled "A Spatial Change Feature-Based Deep Learning Method for Multi-Mineral Segmentation in Micro-CT Rock Images". This work focuses on treating 3D spatial data as sequential data to capture mineralogical transitions more effectively.

### Project Overview
The core objective of this research is to improve multi-class segmentation (Pore, Quartz, Clay, and Feldspar) in Bentheimer sandstone micro-CT scans. By leveraging spatial changes between consecutive slices, the models are designed to recognize patterns that standard 2D U-Nets often miss.

### Models Included:
LSTM U-Net: Integrates ConvLSTM blocks to capture sequential spatial dependencies.

Frame Difference U-Net: Uses the difference between adjacent slices as an additional feature stream.

Two-Stream U-Net: A hybrid approach combining raw image data and spatial change features.

### Repository Structure
spatial_changes_unet.ipynb: The primary Jupyter Notebook containing the end-to-end pipeline:

Data downloading and preprocessing.

Dataset splitting and albumentations augmentation.

Model architectures and training loops.

Evaluation metrics (mIoU, Pixel Accuracy) and Confusion Matrix visualization.

### Requirements & Setup
Environment
We recommend running this notebook on Kaggle or Google Colab to utilize GPU acceleration (T4 or P100 recommended).

Dependencies
The following libraries are required (installed within the notebook):

TensorFlow / Keras

Albumentations (for advanced image augmentation)

Pandas, Numpy (for data handling)

Matplotlib, Seaborn (for visualization)

### Evaluation & Results
The models are evaluated on multi-mineral segmentation tasks using:

Mean Intersection over Union (mIoU)

Normalized Confusion Matrices (Row-wise normalization)

Visual Slice Comparison (Ground Truth vs. Prediction)

The notebook includes a custom visualization function to see how the models perform across different mineral classes in the 3D volume.

## Contact
For questions regarding the methodology or implementation:

Author: Aufaclav Z.K. Frisky, Ridho A. Yusuf (ridhoadiwignyoyusuf@mail.ugm.ac.id

Affiliation: Master’s in Computer Science, University of Gadjah Mada
