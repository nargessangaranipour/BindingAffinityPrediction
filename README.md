# Binding Affinity Prediction

## Overview
This repository contains a convolutional deep learning model designed for predicting the binding affinity between Major Histocompatibility Complex (MHC) proteins and peptides ranging from 9 to 14 amino acids in length. This model demonstrates a significant improvement in the Area Under the Curve (AUC) metric compared to existing models. Furthermore, it uniquely handles peptides of varying lengths (9-14 amino acids), unlike other models which often treat additional amino acids in longer peptides uniformly.

![1](https://github.com/nargessangaranipour/BindingAffinityPrediction/assets/113282317/6479a1fe-088e-459e-90f7-b369d9e29f7c)
## Features
Enhanced Prediction Accuracy: Achieves a higher AUC score, indicating more reliable binding affinity predictions.
Broad Peptide Length Coverage: Accommodates peptides ranging from 9 to 14 amino acids, a notable improvement over other models.
Data-Driven Approach: Utilizes convolutional neural networks, leveraging their ability to extract patterns and features from biological sequences.


## Requirements
- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Seaborn
