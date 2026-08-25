# ACDC-Cardiac-Segmentation
Deep learning-based cardiac MRI segmentation using U-Net and the ACDC dataset.
# Automated Cardiac MRI Segmentation Using U-Net

## Overview

This project develops a deep learning pipeline for automatic
segmentation of cardiac structures from MRI images using a
U-Net architecture.

## Dataset

The project uses the ACDC dataset.

- 1,912 MRI slices
- 100 patients
- 4 segmentation classes
- Image size: 256 × 256

## Classes

| Class | Structure |
|------|-----------|
| 0 | Background |
| 1 | Right Ventricle |
| 2 | Myocardium |
| 3 | Left Ventricle |

## Methodology

MRI Images
↓
Preprocessing
↓
Patient-Level Split
↓
Normalization
↓
U-Net
↓
Segmentation
↓
Dice / IoU Evaluation

## Model

A U-Net encoder-decoder architecture was implemented
using TensorFlow/Keras.

## Results

### Baseline U-Net

| Structure | Dice | IoU |
|---|---:|---:|
| RV | 0.8544 | 0.7458 |
| Myocardium | 0.8463 | 0.7335 |
| LV | 0.9377 | 0.8826 |

Mean Dice: **0.9089**

Mean IoU: **0.8391**

## Experiments

The project includes:

- Baseline U-Net
- Data augmentation
- Error analysis
- Patient-level 5-fold cross-validation

## Repository Structure

...
