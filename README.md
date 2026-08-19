# DeepVesTP

**Interpretable Deep Learning for Vesicular Transport Protein Prediction**

Code repository for the manuscript *DeepVesTP: Interpretable Deep Learning for Vesicular Transport Protein Prediction*.

## Description

This repository contains the implementation used for the DeepVesTP study, including feature preparation, deep learning model training, evaluation, and SHAP-based interpretability analysis.

## Repository Structure

```
DeepVesTP/
├── Models/
│   ├── config.json
│   ├── metadata.json
│   ├── scaler_acc0_9604.pkl
│   └── vtp_cnn_model_acc0_9604_mcc...
├── notebooks/
│   ├── 01_Self_Consistency.ipynb
│   ├── 02_Deep_Learning_Independent_Validation.ipynb
│   ├── 03_10_Cross_Validation.ipynb
│   └── 04_Boundary_Visualization.ipynb
├── Dataset/
│   ├── Pos_Dataset.csv
│   └── Neg_Dataset.csv
├── .gitignore
└── README.md
```

## Notebooks

- **`01_Self_Consistency.ipynb`** — self-consistency evaluation of the model
- **`02_Deep_Learning_Independent_Validation.ipynb`** — independent validation of the deep learning model
- **`03_10_Cross_Validation.ipynb`** — 10-fold cross-validation results
- **`04_Boundary_Visualization.ipynb`** — decision boundary / SHAP-based interpretability visualization

## Model Files

- **`vtp_cnn_model_acc0_9604_mcc...`** — trained CNN model (accuracy 0.9604)
- **`scaler_acc0_9604.pkl`** — feature scaler used for preprocessing
- **`config.json`** / **`metadata.json`** — model configuration and metadata

## Installation

Clone the repository:

```bash
git clone https://github.com/Tayyabaakmal/DeepVesTP.git
cd DeepVesTP
```

> **Note:** A `requirements.txt` will be added listing exact package versions. Key dependencies include Python, a deep learning framework (PyTorch/TensorFlow — specify which), scikit-learn, and SHAP — see the notebooks' import cells for the full list.

## Usage

Open any notebook in the `notebooks/` folder to reproduce the corresponding analysis:

```bash
jupyter notebook notebooks/01_Self_Consistency.ipynb
```

Trained model artifacts are located in `Models/` and can be loaded directly for inference without re-training.

## Dataset

Protein sequences were obtained from UniProtKB and processed as described in the manuscript. The complete dataset is not redistributed in this repository due to size/licensing constraints. See the manuscript's Methods section for accession details and filtering criteria.

## Citation

If you use this code, please cite:

```bibtex
@article{yourname_deepvestp,
  title={DeepVesTP: Interpretable Deep Learning for Vesicular Transport Protein Prediction},
  author={Your Name(s)},
  journal={Journal Name},
  year={2026}
}
```

## License

License to be added.

## Contact

For questions, please open an issue on this repository or contact [your email].
