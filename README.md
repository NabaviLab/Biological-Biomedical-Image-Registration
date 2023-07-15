# Biological-Biomedical-Image-Registration

This repository contains the implementation of our novel image registration method, as described in our paper titled "3D Biological/Biomedical Image Registration with enhanced Feature Extraction and Outlier Detection". Our method outperforms other state-of-the-art techniques in various scenarios and demonstrates superiority across various image quality metrics.

## Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Datasets](#datasets)

## Introduction

Our image registration method tackles the challenges posed by distortions and transformations and proves effective in registering images with high reliability and visual quality. The method has shown impressive performance on complex 3D multiplex microscopy and 3D MRI images. 

## Installation

To install and run this project, you will need Python 3.6 or later. Clone the repository and install the necessary requirements:

```bash
git clone https://github.com/NabaviLab/Biological-Biomedical-Image-Registration
cd 3D-Biological-Biomedical-Image-Registration
```
And to. install libraries, please follow the below command in the first cell of the Google Colab/Jupyter Notebook:
```bash
!pip install opencv-python-headless numpy torch torchvision pillow scipy pandas matplotlib seaborn plotly scikit-image psutil scikit-learn
```

## Usage

This repository contains two `.ipynb` (Jupyter Notebook) files:
1. `ResNet 50 Fine Tuning.ipynb`: This file allows you to fine-tune the ResNet-50 model based on your dataset.
2. `3D Biological/Biomedical Image Registration.ipynb`: This is the main registration file where the registration algorithm is implemented.

To use these notebooks, follow the steps below:
Navigate to the repository folder after installation.
```bash
cd 3D-Biological-Biomedical-Image-Registration
```

## Datasets
You can use any 3D biological/biomedical images for registration. However, our model performs best with 3D multiplex microscopy and 3D MRI images. For your convenience, we provide the "CUMC12" dataset, which is synthesised based on known transformations. This dataset is ideal for testing the algorithm. The "CUMC12" dataset we used in our paper is publicly available:

```bash
https://continuousregistration.grand-challenge.org/data/
```

In case you use the "CUMC12" dataset, please follow the citation guidelines below:

```bash
@article{klein2009evaluation,
  title={Evaluation of 14 nonlinear deformation algorithms applied to human brain MRI registration},
  author={Klein, Arno and Andersson, Jesper and Ardekani, Babak A and Ashburner, John and Avants, Brian and Chiang, Ming-Chang and Christensen, Gary E and Collins, D Louis and Gee, James and Hellier, Pierre and others},
