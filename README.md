# NSAP Scheme Eligibility Prediction Using Machine Learning

This project was developed as part of the **AICTE + IBM SkillsBuild + Edunet Foundation Internship (2025)**.  
It leverages machine learning to classify beneficiaries under India's **National Social Assistance Programme (NSAP)** into the most appropriate welfare schemes using district-level demographic data.

---

## Objective

To automate the classification of welfare scheme eligibility under NSAP using a data-driven approach.  
The model predicts eligibility for the following social assistance schemes:

- **IGNOAPS** — Indira Gandhi National Old Age Pension Scheme  
- **IGNWPS** — Indira Gandhi National Widow Pension Scheme  
- **IGNDPS** — Indira Gandhi National Disability Pension Scheme  

---

## Problem Statement

Manual eligibility verification for NSAP schemes is time-consuming, inconsistent, and difficult to scale across large populations.  
This project addresses the challenge by applying supervised machine learning to predict eligibility based on gender, caste, Aadhaar access, and mobile availability data.

---

## Proposed Solution

The system utilizes a Random Forest classifier trained on demographic and beneficiary-related features to predict the correct scheme class for an applicant.  
The model is integrated within a Jupyter Notebook hosted on IBM Watson Studio under IBM Cloud, following the complete ML pipeline: data preprocessing, model training, evaluation, and reporting.

---

## Technologies Used

- **IBM Cloud (Lite Account)**
  - Watson Studio / Cloud Pak for Data
  - IBM Object Storage for dataset handling

- **Languages & Libraries**
  - Python 3.11
  - Scikit-learn (RandomForestClassifier)
  - Pandas, NumPy, Matplotlib
  - Jupyter Notebook

---

## Dataset Information

- **File Name**: `nsapallschemes.csv`  
- **Records**: 2156 rows × 16 columns  
- **Features**:  
  - Gender-based counts (`totalmale`, `totalfemale`, `totaltransgender`)  
  - Social categories (`totalsc`, `totalst`, `totalobc`, `totalgen`)  
  - Aadhaar and mobile penetration (`totalaadhaar`, `totalmobilenumber`)  
  - State and district codes

> *Note: This dataset was provided as part of the IBM SkillsBuild Internship. It is not publicly hosted on Kaggle.*

---

## Model Overview

- **Algorithm**: Random Forest Classifier  
- **Data Split**: 80% Training / 20% Testing  
- **Accuracy Achieved**: **97.2%**

### Evaluation Metrics

| Metric        | Score     |
|---------------|-----------|
| Accuracy      | 97.2%     |
| Precision     | 96–99%    |
| F1 Score      | >97%      |
| Confusion Matrix | Very low misclassification across classes |

The model demonstrates strong generalization and high confidence in scheme classification across all three labels.

---

## How It Works

1. **Data Ingestion**: Reads `.csv` data directly from IBM Object Storage  
2. **Preprocessing**: Feature selection, null checks, label encoding  
3. **Modeling**: Fits a Random Forest Classifier with default hyperparameters  
4. **Evaluation**: Prints classification report, confusion matrix, and accuracy score  
5. **Output**: Displays predictions and model evaluation summary in notebook

---

## Project Files

- `NSAP_ML_Notebook.ipynb` — Main notebook with all development steps  
- `ProjectPresentation.pptx` — Slide deck for submission  
- `LICENSE` — MIT License with custom attribution  

---

## Author

**Swati Upadhyay**  
BCA Student, Vaugh Institute of Agriculture Engineering and Technology  
IBM SkillsBuild Cloud & AI Intern – 2025 Cohort  

📧 uswati1123@gmail.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/swati-upadhyay-b042241a4/)

---

## Repository Status

✅ **Project Completed and Submitted** under AICTE–IBM–Edunet Internship  
🗓️ Submission Deadline: August 4, 2025  
☁️ Developed entirely on IBM Cloud (Watson Studio)

---

## Licensing

This project is released under the [MIT License](./LICENSE).  
**Reproduction, redistribution, or submission without author attribution is strictly prohibited.**
