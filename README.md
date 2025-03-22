ISIC 2024 - Skin Cancer Detection with 3D-TBP

Kaggle competition:
https://www.kaggle.com/competitions/isic-2024-challenge

Image Model (CNN):
A convolutional neural network (CNN) is used to process skin lesion images.
-Three convolutional layers (with 25, 50, and 100 filters),
-Max pooling and dropout layers after the first two convolutional layers,
-A flatten layer followed by batch normalization,
-Three fully connected (dense) layers with dropout,
-A final dense layer with a sigmoid activation to output a probability.

Metadata is processed using feature engineering, including:
-Filling missing values,
-One-hot encoding of categorical variables,
-Normalization of numerical features.

Metadata Models:
Models trained on clinical metadata (e.g. age, sex, lesion size, and 3D-TBP features):
Two XGBoost models:
-One trained on the original dataset,
-One trained on a SMOTE-resampled version to address class imbalance.
-One CatBoostClassifier model, designed to handle categorical variables and missing values.



Ensemble Strategy:
Predictions from the image model and the metadata models are combined using an ensemble method (e.g. averaging or stacking) to improve final performance.
