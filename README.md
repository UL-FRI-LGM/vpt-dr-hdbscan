# Interactive Visualization of High-Dimensional Voxel Features in Volumetric Path Tracing using Dimensionality Reduction and HDBSCAN
A repository containing code developed as part of the Bachelor thesis at the University of Ljubljana, Faculty of Computer and Information Science by Tilen Smrdel.

## Abstract
This work introduces an interactive visualization framework for exploring complex volumetric microscopy data, using multi-dimensional feature extraction and dimensionality reduction to improve structural analysis. Each voxel is assigned an 11-dimensional feature vector to capture both local and global context. After uniform sampling, we apply UMAP and t-SNE for dimensionality reduction, followed by HDBSCAN for density-based clustering. The resulting clusters are mapped back to the original volume to construct an interactive transfer function, with Gaussian blobs representing cluster centers. Expert evaluation of troponin-labeled cardiomyocytes shows that this analysis offers greater sensitivity in detecting treatment-induced structural remodeling than standard visual inspection. Non-treated samples display higher morphological heterogeneity, with multiple small regions of varying intensity, while treatment with 500 nM carfilzomib for 24 hours leads to fewer, more dominant phenotypic states characterized by localized protein clustering and nuclear enlargement. Our results demonstrate that this unbiased, quantifiable workflow successfully reveals treatment-associated structural changes and protein redistributions that remain undetected in conventional 2D immunofluorescence evaluation.

## vpt-dr-hdbscan
A web application to compute and visualize clusters of structures from microscopy image stacks.

The volumetric visualization is created from 2D image stacks provided by the user, collected from digital microscopes such as the Operetta. The image data is then prepared and processed to compute clusters based on any observed structures in the image data. These are then visualized, the visualization can be manipulated by the user.

This clustering works on any microscopy image data, works better on some cells than others.

The image stacks were provided by the University of Ljubljana, Faculty of Farmacy

## Description of code workflow
