# NSAP Scheme Eligibility Prediction using ML

This project was developed as part of the **AICTE + IBM SkillsBuild + Edunet Foundation Internship (2025)**.  
It uses Machine Learning to classify the correct **NSAP (National Social Assistance Programme)** scheme based on district-wise demographic features.

---

## Objective

To build a classification model that predicts which social security scheme a beneficiary is eligible for:
- `IGNOAPS` – Old Age Pension
- `IGNWPS` – Widow Pension
- `IGNDPS` – Disability Pension

---

## Technologies Used

- IBM Cloud (Cloud Pak for Data / Watson Studio)
- Python (Pandas, Scikit-learn)
- Jupyter Notebooks
- Data Visualization
- RandomForestClassifier

---

## Dataset Used

- **Name**: `nsapallschemes.csv`
- **Source**: Kaggle (provided by AICTE/IBM)
- **Records**: 2156 rows × 16 columns
- **Features**: Beneficiary counts by gender, caste, Aadhaar availability, mobile access, etc.

---

## Model Details

- **Algorithm**: Random Forest Classifier
- **Training Split**: 80% training / 20% testing
- **Accuracy**: 97.2%
- **Metrics Used**: Accuracy, Precision, F1-score, Confusion Matrix

---

## Results

| Metric        | Score |
|---------------|--------|
| Accuracy      | 97.2%  |
| Precision     | 96–99% |
| F1-Score      | 97%+   |

The model performs excellently across all three scheme types.

---

## Files Included

- `NSAP_ML_Notebook.ipynb` – Main Jupyter Notebook
- `nsapallschemes.csv` – Dataset
- `NSAP_Eligibility_Prediction_Report.pdf` – Notebook exported as PDF
- `ProjectPresentation.pptx` – Final presentation slides
- `LICENSE` – MIT License with custom attribution

---

## Disclaimer

> This project was submitted by **Swati Upadhyay** as part of the IBM SkillsBuild Internship.  
> Copying, redistributing, or submitting without proper attribution is prohibited.

---

## Author

**Swati Upadhyay**  
AI & Cloud Intern | BCA Student | IBM SkillsBuild Intern  
 `uswati1123@gmail.com`  
 [LinkedIn Profile](https://www.linkedin.com/in/swati-upadhyay-b042241a4/)

---

## Status

**Project Completed** and Submitted  
IBM Cloud Workspace used  
Submission Deadline: 4th August 2025

