# NearEarthObject-Analysis-Classification-Project
Introduction
This project involves analyzing the Nearest Earth Objects (1910-2024) dataset. The analysis focuses on understanding key features such as object size, velocity, miss distance, and the hazardous nature of these objects. The dataset is cleaned, visualized, and used to build a classification model to predict whether an object is hazardous or not.

Dataset Information
The dataset contains information about near-Earth objects (NEOs) from 1910 to 2024. The columns in the dataset include:

neo_id: Unique identifier for the near-Earth object.
name: Name of the near-Earth object.
absolute_magnitude: The absolute magnitude of the NEO.
estimated_diameter_min: Estimated minimum diameter of the NEO (in kilometers).
estimated_diameter_max: Estimated maximum diameter of the NEO (in kilometers).
orbiting_body: Primary celestial body that the object is orbiting.
relative_velocity: The velocity of the NEO relative to Earth (in km/h).
miss_distance: The distance at which the object will miss Earth (in kilometers).
is_hazardous: Indicator if the NEO is classified as hazardous.
Data Cleaning and Preprocessing
The dataset underwent several cleaning steps:

Handling missing values: Columns such as absolute_magnitude, estimated_diameter_min, and estimated_diameter_max had missing values which were filled with their respective means.
Outlier treatment: Outliers were replaced with mean values to minimize their impact on model training.
Feature engineering: New columns for year and object code were extracted from the name column for further analysis.
Label encoding: Categorical columns such as orbiting_body and is_hazardous were encoded using LabelEncoder.
Data Analysis and Visualizations
Several analysis questions were explored, such as:

Distribution and statistics for absolute_magnitude, estimated_diameter_min, estimated_diameter_max, and relative_velocity.
Trends of hazardous objects by year and orbiting body.
Relationship between object size and hazard classification.
Visualizations such as histograms, box plots, and pie charts were used to analyze the data distribution and trends.

Modeling and Evaluation
A Random Forest Classifier was used to predict whether an NEO is hazardous or not.

Steps:
The dataset was split into training and testing sets (80% training, 20% testing).
The model was trained on the training set.
The model's accuracy was evaluated on both the training and test sets.
Model Performance:
Training Accuracy: Achieved high accuracy on the training set.
Test Accuracy: The model performed well on unseen data.
Classification Report: Precision, recall, and F1-score were computed to assess the model's performance on the test set.
