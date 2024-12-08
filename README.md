# Binding Affinity Prediction

This project focuses on predicting peptide-MHC binding affinity using a deep learning approach. It leverages convolutional neural networks (CNNs) to encode and analyze sequence data, enabling accurate predictions in the context of peptide-MHC interactions. This model demonstrates a significant improvement in the Area Under the Curve (AUC) metric compared to existing models. Furthermore, it uniquely handles peptides of varying lengths (9-14 amino acids), unlike other models which often treat additional amino acids in longer peptides uniformly. The project is implemented in Python using TensorFlow/Keras.
![1](https://github.com/nargessangaranipour/BindingAffinityPrediction/assets/113282317/0ddffa6a-2430-435b-b9fa-8f715e3aa6ad)

## Features

- **Sequence Encoding**: One-hot encoding for peptide and MHC sequences.
- **Model Architecture**: CNN-based architecture designed to process sequence inputs.
- **Class Imbalance Handling**: Incorporates class weights to balance datasets.
- **Visualization**: Includes plots for label distribution, training loss, and ROC curves.
- **Performance Metrics**: Calculates accuracy, precision, recall, F1-score, and AUC.
- **Hardware Optimization**: Supports GPU acceleration and multi-threaded data processing.

## File Structure

- **Notebook**: `Binding Affinity Prediction.ipynb` contains all code for the project.

## Requirements

- **Python Packages**:
  - `tensorflow`
  - `keras`
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `sklearn`
- **System Requirements**:
  - GPU support recommended for faster training (e.g., NVIDIA CUDA).
  - Multi-core CPU for efficient data handling.

## Usage

### 1. Clone the Repository
```
git clone https://github.com/nargessangaranipour/BindingAffinityPrediction
cd BindingAffinityPrediction
```

### 2. Prepare Data
Ensure the dataset is located in the `data/` directory. The dataset should include:
- A column for MHC sequences.
- A column for peptide sequences.
- A label column indicating binding affinity.

### 3. Run the Notebook
Launch the Jupyter notebook and execute the cells sequentially:
```
jupyter notebook
```
Open `Binding_Affinity_Prediction.ipynb` and run all cells.

## Outputs

- **Model Artifacts**: Saved in the `dist/` directory after each epoch.
- **Plots**:
  - Label distribution.
  - Training loss vs. epochs.
  - ROC curves.
- **Metrics**: Reported as a summary table in the notebook.
- **Model and Results Visuals**: ![ca73486c-0397-49af-a868-29c17b127145](https://github.com/user-attachments/assets/5c4c756d-1e6d-4181-a84d-5be09d29e577)


## Highlights

- **Data Generators**: Reduce memory usage during training.
- **Class Weighting**: Mitigates class imbalance issues.
- **Evaluation Metrics**: Comprehensive performance evaluation for the predictive model.

## Biological Relevance
Binding affinity predictions are critical for understanding immune responses and designing vaccines or therapeutics. By modeling peptide-MHC interactions, this project supports advancements in:

- **Immunotherapy**: Identifying candidates for cancer treatment and autoimmune disease management.
- **Vaccine Design**: Developing effective vaccines by predicting strong peptide binders.
- **Drug Discovery**: Enhancing the selection of therapeutic peptides with high binding affinities.

### References
1. [Schatz DG, et al., "Molecular biology of MHC molecules."](https://www.ncbi.nlm.nih.gov/pubmed/)
2. [Parker KC, et al., "Peptide binding specificity of MHC class I molecules."](https://www.ncbi.nlm.nih.gov/pubmed/)

## Potential Applications
This project can be extended or adapted for:
- Predicting other sequence-based biological interactions.
- Drug discovery and immunotherapy research.
- Large-scale analysis of sequence data in genomics.

## Contributions
Feel free to contribute by submitting pull requests or issues.


