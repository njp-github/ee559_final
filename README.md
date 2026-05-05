# ee559_final
Code and instructions to run scripts for EE 559 (Sp2026) Final Project by Rama Chandra Bhogasamudram and Neil Patel.

### Package requirements:
- nibabel
- numpy, pandas, matplotlib
- pytorch
- pytorch-3dunet (conda install -c conda-forge pytorch-3dunet)

# Fetal Brain Segmentation and Age Prediction — Notebook Overview

1. Extract tissue volumes from pre-annotated segmentation masks → Ridge regression age prediction (baseline)
2. Train 3 segmentation models on T2w images:
   - **Vanilla 3D CNN** (encoder-only, small)
   - **Vanilla 3D CNN with Instance Norm**
   - **3D UNet** Just to benchmark with popular and pre-defined architecture
3. Loss: `CombinedLoss = ce_w·CrossEntropy + (1−ce_w)·SoftDiceLoss` (background ignored)
4. Evaluation: per-class Dice score + mean Dice (foreground) + voxel accuracy (without background)
5. End-to-End: Age Prediction from Predicted Segmentation of MRI
