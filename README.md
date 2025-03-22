ISIC 2024 - Skin Cancer Detection with 3D-TBP

https://www.kaggle.com/competitions/isic-2024-challenge

This project is a submission for the ISIC 2024 Challenge, focusing on classifying skin lesions as malignant or benign. The approach combines both metadata and image-based analysis. Key features of the pipeline include:

Separate handling of benign and malignant cases due to class imbalance.

Creation of multiple models trained on different benign subsets for ensemble learning.

Use of CNNs (Convolutional Neural Networks) for image classification and XGBoost for metadata analysis.

Image data is read and resized from HDF5 files for efficient processing.
