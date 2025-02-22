H1N1 and Seasonal Vaccine Prediction
Overview
This project aims to predict vaccine uptake for H1N1 and Seasonal Influenza using machine learning techniques. The dataset contains demographic, behavioral, 
and medical factors influencing vaccine decisions. The goal is to build a robust classification model to help health organizations target vaccination campaigns effectively.

Business and Data Understanding
Stakeholder Audience
The key stakeholders include:
Public health officials – To design better vaccination awareness campaigns.
Medical researchers – To analyze factors affecting vaccine uptake.
Government agencies – To allocate resources effectively for vaccination drives.

Dataset Choice
The dataset comes from the National 2009 H1N1 Flu Survey (NHFS) and includes:
Demographics – Age, gender, employment, etc.
Health-related factors – Chronic illnesses, doctor recommendations.
Behavioral aspects – Trust in vaccines, media influence.
Vaccine uptake labels – Whether an individual took the H1N1 and seasonal flu vaccine.
Modeling
The project uses a Decision Tree Classifier with the following configurations:

Handling class imbalance: class_weight="balanced"
Hyperparameter tuning: Grid search for max_depth, criterion, and min_samples_split
Feature Engineering: Encoding categorical variables, handling missing values.

Evaluation
I evaluated the models using:

Accuracy – Measures overall correctness.
Precision & Recall – Important due to class imbalance.
AUC-ROC – Measures classification performance for imbalanced data.

Results:
H1N1 Vaccine Model:
Test Accuracy: 84.05%
Precision: 0.68 (for positive class)
Recall: 0.40
Seasonal Flu Vaccine Model:
Test Accuracy: 76.68%
Precision: 0.76
Recall: 0.73

Conclusion
Doctors' recommendation and trust in vaccines play a key role in vaccine uptake.
The decision tree performed well but struggled with recall for the H1N1 vaccine group.
Class imbalance impacted model performance, but class weighting improved fairness.
Further improvement can be achieved using ensemble methods like Random Forest.
