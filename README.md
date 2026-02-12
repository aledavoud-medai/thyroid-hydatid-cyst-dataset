# Global Dataset of Thyroid Hydatid Cyst (THC) Cases

## Overview

This repository contains a curated and cleaned dataset of all published cases of **Thyroid Hydatid Cyst (THC)** reported worldwide.

The dataset includes demographic, clinical, radiological, and treatment-related variables extracted from published case reports and case series.

Total number of patients: **75**

This repository aims to provide a structured dataset for future epidemiological, clinical, and statistical analysis of this rare condition.

---

## Dataset Description

After preprocessing and cleaning, the dataset contains 18 variables:

- `patient_id` – Unique identifier
- `year` – Year of reported case
- `rural` – Rural residence (0 = No, 1 = Yes, NaN = Not reported)
- `gender` – 0 = Male, 1 = Female
- `age` – Age in years
- `country` – Country of case report
- `duration_years` – Disease duration before diagnosis
- `symptom_type` – Original reported symptoms
- `cyst_size_mm` – Cyst size in millimeters
- `Serology` – Hydatid serology (1 = Positive, 0 = Negative)
- `follow_up_outcome` – Post-treatment complication (1 = Yes, 0 = No)
- `surgery` – Surgical treatment performed (1 = Yes)
- `medication` – Antiparasitic medication administered (1 = Yes)
- `has_mass` – Neck mass present
- `has_pulmonary` – Pulmonary symptoms present
- `has_digestive` – Digestive symptoms present
- `right_lobe` – Right thyroid lobe involvement
- `left_lobe` – Left thyroid lobe involvement

Missing values are represented as `NaN`.

---

## Data Processing

The following preprocessing steps were performed:

1. Replacement of non-reported values ("N/d") with NaN  
2. Type conversion of numerical columns to appropriate numeric formats  
3. Binary encoding of:
   - living location(rural, urban)
   - gender(male, female)
   - Treatment modalities (surgery, medication)
   - Symptoms
   - Cyst location (right/left lobe)
4. Logical sanity checks for:
   - Age range
   - Cyst size range
   - Missing value consistency

The dataset is fully reproducible using the provided Jupyter Notebook.

---

## Repository Structure
- `thyroid_hydatid_cyst.csv` – Original raw dataset before preprocessing
- `thyroid_hydatid_cyst_cleaned.csv` – Final cleaned dataset  
- `analysis.ipynb` – Data cleaning and preprocessing notebook  
- `README.md` – Project documentation  

---

## Research Use

This dataset is intended for:

- Epidemiological studies  
- Clinical pattern analysis  
- Treatment outcome evaluation  
- Statistical modeling  

If used in academic work, please cite the original case reports.

---

## Author

Independent data curation and preprocessing for academic and research purposes.
