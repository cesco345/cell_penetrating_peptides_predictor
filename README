# Cell-Penetrating Peptide (CPP) Predictor Project Summary

## Project Overview
This project aimed to develop a machine learning model to predict whether a given peptide sequence is a cell-penetrating peptide (CPP) or not. CPPs are short peptides that can traverse cell membranes and potentially deliver molecular cargo into cells, making them valuable in drug delivery and biotechnology.

## Data Preparation and Feature Extraction
1. We started with a small dataset of 30 peptide sequences (15 CPPs and 15 non-CPPs).
2. Features were extracted based on amino acid composition and physicochemical properties.
3. The dataset was split into training (24 samples) and test (6 samples) sets.

## Initial Model Development
1. We implemented three types of models:
   - Feedforward Neural Network (FFN)
   - Convolutional Neural Network (CNN)
   - Recurrent Neural Network (RNN)
2. These models showed varying performance, with potential overfitting due to the small dataset.

## Feature Selection and Model Refinement
1. We performed feature selection using SelectKBest, reducing from 15 to 5 features.
2. The selected features were: 7, 8, 9, 10, and 14.
3. We experimented with simpler models like Logistic Regression and Decision Trees.

## Hyperparameter Tuning
We used GridSearchCV to tune hyperparameters for our best-performing model.

## Final Model and Analysis
1. A Random Forest classifier was chosen as the final model due to its good performance and interpretability.
2. Feature importance analysis revealed that Feature 14 was by far the most important, followed by Features 9, 8, and 7.

## Simple Decision Tree Model
We created a simple decision tree using the top two features (14 and 9), which provided easily interpretable rules:
- If Feature 14 ≤ 0.70, classify as non-CPP
- If Feature 14 > 0.70:
  - If Feature 9 ≤ 0.04 or > 0.09, classify as CPP
  - If 0.04 < Feature 9 ≤ 0.09, classify as non-CPP

## Visualizations and Interpretations
1. We created decision boundary plots to visualize how the model separates CPPs from non-CPPs.
2. Feature importance was visualized using both Mean Decrease in Impurity and Permutation Importance methods.

## Key Findings
1. Feature 14 (likely representing a key physicochemical property) is crucial for CPP classification.
2. There's a non-linear relationship between Features 14 and 9 in determining CPP status.
3. A simple rule-based classifier using just two features can provide reasonable performance.

## Limitations and Future Work
1. The small dataset size (30 samples) limits the model's generalizability.
2. Further data collection, focusing on the identified important features, would be beneficial.
3. Consultation with domain experts is needed to interpret the biological significance of the findings.

## Next Steps
1. Identify the exact peptide properties that the important features represent.
2. Validate the model's findings with peptide science experts.
3. Collect more data, especially around the identified decision boundaries.
4. Investigate peptides that are near the decision boundaries for potential insights.
5. Consider developing a more robust model with a larger dataset while maintaining interpretability.

This project demonstrates the potential of machine learning in predicting cell-penetrating peptides, while also highlighting the importance of combining data-driven approaches with domain expertise in bioinformatics research.
