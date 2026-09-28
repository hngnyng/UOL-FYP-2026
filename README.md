# Mammogram Classification Using Deep Learning

This project investigates binary classification of mammogram
abnormalities as benign or malignant using the CBIS-DDSM dataset.

The implemented models include:

- A custom convolutional neural network trained from scratch
- A frozen ResNet50 feature extractor
- A frozen VGG16 feature extractor
- Hyperparameter-tuned classification models

## Dataset

This project uses the Curated Breast Imaging Subset of the Digital
Database for Screening Mammography (CBIS-DDSM).

The dataset is not included in this repository because of its size.
It can be obtained from The Cancer Imaging Archive:

https://www.cancerimagingarchive.net/collection/cbis-ddsm/

Dataset citation:

Sawyer-Lee, R., Gimenez, F., Hoogi, A., & Rubin, D. (2016).
Curated Breast Imaging Subset of Digital Database for Screening
Mammography (CBIS-DDSM). The Cancer Imaging Archive.
https://doi.org/10.7937/K9/TCIA.2016.7O02S9CY

The notebook expects the data to be arranged approximately as:

```text
CBISDDSM-AWSAF/
├── csv/
│   ├── dicom_info.csv
│   ├── mass_case_description_train_set.csv
│   ├── calc_case_description_train_set.csv
│   ├── mass_case_description_test_set.csv
│   └── calc_case_description_test_set.csv
└── jpeg/
    └── ...
```

Update `localPath` in the notebook if the dataset is stored elsewhere.

## Installation

Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1 
