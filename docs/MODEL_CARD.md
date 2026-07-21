# Model Card

## Intended use

Academic classification of Breast Cancer Wisconsin (Diagnostic) records as malignant or benign.

## Not intended for

Clinical diagnosis, treatment decisions, screening or use with patient data outside the supplied academic dataset.

## Data

569 observations and 30 numerical predictors after removal of the identifier and empty column.

## Final model

A one-dimensional convolutional neural network with two convolutional layers, batch normalisation, max pooling, dropout and fully connected layers.

## Evaluation

The untouched test set contains 114 records. The improved model achieved:

- Accuracy: 0.9649
- Malignant precision: 0.9524
- Malignant recall: 0.9524
- Malignant F1: 0.9524
- Specificity: 0.9722
- ROC-AUC: 0.9964
- False negatives: 2
- False positives: 2

## Main limitations

Small dataset, no external validation, no probability calibration study, tabular inputs rather than raw images, and no clinical or regulatory assessment.
