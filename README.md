# Alzheimer-s-Disease-Classification

Dataset Link: https://www.kaggle.com/datasets/aryansinghal10/alzheimers-multiclass-dataset-equal-and-augmented?resource=download

Undersampled dataset, used during the training (derived from the original): https://drive.google.com/file/d/1LauG-A8BMNlEME3CRPQRbmaVMh7ZHe2f/view?usp=drive_link

# Implementation & Reproducibility Notes
This repository contains a clean re-implementation of the models presented in the published paper.

While the proposed method is implemented as described in the manuscript, the baseline models (InceptionV3 and MobileNetV2) may not exactly reproduce the performance reported in the paper. Potential sources of variation include the absence of earlier class undersampling strategies used during manuscript experimentation and minor variations in training setup or hyperparameters.

# Learning Rate Clarification
During reproduction, it was observed that the learning rate reported in the manuscript (0.001) does not yield the performance described in the experimental results. After careful re-evaluation of the training configuration, the effective learning rate used during experimentation was 0.0001. The value 0.001 appears to have been reported mistakenly during manuscript preparation. The implementation in this repository reflects the correct learning rate (0.0001) used to obtain the published results. The primary contribution and proposed method remain consistent with the description in the published work.

The purpose of this repository is to provide a clean, maintainable, and reproducible implementation of the framework, along with clarification where necessary to ensure transparency.

# Repository Update (Baseline Model Revision)
An updated version of the codebase has been uploaded to improve the implementation of the baseline architectures InceptionV3 and MobileNetV2. These models are included only for comparative evaluation and are not part of the proposed method or main contribution of the paper. The updated implementation improves code clarity and consistency in the training pipeline while maintaining the overall experimental setup. No changes were made to the proposed framework or the core methodology described in the manuscript. The update only affects the baseline model implementations used for comparison.
