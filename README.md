# Alzheimer's Disease Detection using Machine Learning

## Project Overview

This project aims to develop a machine learning model to classify the stages of Alzheimer's Disease (AD) using the OASIS dataset. The model leverages the Random Forest algorithm due to its high accuracy and robustness in classification tasks. The project includes data preprocessing, feature selection, model training, and evaluation.

### Authors
- Fleur LAURENS
- Laura SAYAPHOMMY
- Zyad TAOUIL
- M2 IKSEM

## Problem Explanation and Task Identification

The primary objective is to classify patients into different stages of dementia based on the Clinical Dementia Rating (CDR) attribute. The stages are:
- 0: No dementia
- 0.5: Very mild AD
- 1: Mild AD
- 2: Moderate AD
- 3: Severe AD

## Dataset Description

The project uses two datasets from OASIS:
1. **oasis_cross-sectional**: 436 rows and 12 columns
2. **oasis_longitudinal**: 373 rows and 15 columns

### Demographics Information:
- **M.F**: Gender
- **Hand**: Handedness (all subjects were right-handed, so this column was dropped)
- **Age**: Age in years
- **EDUC**: Years of education (range: 1 to 23)
- **SES**: Socioeconomic status (1 = highest, 5 = lowest)

### Clinical Information:
- **MMSE**: Mini-Mental State Examination score (range: 0 to 30)
- **CDR**: Clinical Dementia Rating
- **eTIV**: Estimated Total Intracranial Volume (mm³)
- **nWBV**: Normalized Whole Brain Volume (ratio)
- **ASF**: Atlas Scaling Factor (ratio)

## Data Preparation

### Steps Taken:
1. Merging `oasis_cross-sectional` and `oasis_longitudinal` datasets.
2. Dropping irrelevant columns (e.g., MRI ID, Group, Visit).
3. Renaming and dropping columns with null values.
4. One-hot encoding for categorical data (e.g., gender).
5. Label encoding for CDR and SES.
6. Normalizing the data to standardize values.

After cleaning, the final dataset comprised 570 rows and 10 columns.

## Model Implementation

### Random Forest Algorithm
Random Forests are used due to their ensemble nature, which reduces overfitting by aggregating the results of multiple decision trees. Key features include:
- High accuracy and robustness
- Reduced variance and bias
- Flexibility in handling various data types

### Advantages:
- Accurate predictions with low bias and variance
- Reduced overfitting

### Disadvantages:
- Performance may decline with a large number of irrelevant variables

### Ensemble Methods
The project also explores ensemble methods like Voting Classifier, combining:
- Random Forest
- Gradient Boosting
- KNeighbors (with and without SVC)

## Results and Analysis

The Random Forest algorithm provided accurate predictions with reduced bias and variance, proving effective for the classification of Alzheimer's Disease stages. However, the lack of data might have impacted the performance of the algorithm.

## Conclusion

The project successfully developed a machine learning model to classify Alzheimer's Disease stages using the Random Forest algorithm. The model's performance was compared with other ensemble methods, highlighting the effectiveness and limitations of each approach.

## Future Work
- Incorporate additional datasets to improve model performance.
- Explore other machine learning algorithms and ensemble methods.
- Conduct further feature engineering to enhance model accuracy.

## Acknowledgments

We thank the OASIS project for providing the datasets and the M2 IKSEM program for supporting this research.

---
