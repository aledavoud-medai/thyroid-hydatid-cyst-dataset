# Thyroid Hydatid Cyst Dataset and Analysis

## Overview
This repository contains a curated dataset and statistical analysis of all reported cases of **thyroid hydatid cyst (THC)** published in the medical literature worldwide.

The project includes data collection, cleaning, and exploratory statistical analysis aimed at providing a structured resource for future clinical and epidemiological studies.

---

## Repository Structure

thyroid-hydatid-cyst-dataset/
│
├── data/ # Original extracted data (uncleaned) and cleaned and standardized dataset
│
├── notebooks/ # Data analysis notebooks and visualizations
│
├── results/ # Generated tables and statistical outputs
│
└── README.md
---

## Dataset Description

After preprocessing and cleaning, the dataset contains 18 variables:

patient_id – Unique identifier
year – Year of reported case
rural – Rural residence (0 = No, 1 = Yes, NaN = Not reported)
gender – 0 = Male, 1 = Female
age – Age in years
country – Country of case report
duration_years – Disease duration before diagnosis
symptom_type – Original reported symptoms
cyst_size_mm – Cyst size in millimeters
Serology – Hydatid serology (1 = Positive, 0 = Negative)
follow_up_outcome – Post-treatment complication (1 = Yes, 0 = No)
surgery – Surgical treatment performed (1 = Yes)
medication – Antiparasitic medication administered (1 = Yes)
has_mass – Neck mass present
has_pulmonary – Pulmonary symptoms present
has_digestive – Digestive symptoms present
right_lobe – Right thyroid lobe involvement
left_lobe – Left thyroid lobe involvement
Missing values are represented as NaN.
---

## Data Processing

Data preparation involved:

- Removal of duplicates
- Standardization of variable formats
- Handling missing values
- Unit normalization
- Creation of analysis-ready variables
---

## Statistical Analysis

Statistical analyses were performed using Python.

Methods include:

- Descriptive statistics
- Non-parametric tests
- Correlation analysis
- Data visualization

All analysis workflows and figures are available in:\notebooks

## Results

Generated tables and statistical outputs are stored in:\result
Figures are embedded within the analysis notebooks.

---

## Reproducibility

To reproduce the analysis:

1. Clone the repository:

git clone https://github.com/aledavoud-medai/thyroid-hydatid-cyst-dataset.git

2. Install required Python packages:
pip install pandas numpy scipy matplotlib seaborn jupyter

3. Open the notebooks:
jupyter notebook
---

## Intended Use

This repository is intended for:

- Clinical research
- Epidemiological studies
- Medical data science practice
- Educational purposes

---

## Author

Medical researcher and physician interested in clinical data analysis and rare disease datasets.

---

## License

This project is shared for academic and research purposes.
Please cite appropriately if used in scientific work.