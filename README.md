# **NearEarthObject-Analysis-Classification-Project**

## **Introduction**

This project focuses on the analysis of near-Earth objects (NEOs) using the dataset spanning from 1910 to 2024. The aim is to explore key features such as object size, velocity, miss distance, and hazard classification to predict whether a near-Earth object is potentially hazardous. This project involves data cleaning, feature engineering, visualization, and building a classification model to make these predictions.

## **Dataset Information**

The dataset contains detailed information about near-Earth objects (NEOs), including their characteristics and orbit information. Below are the key columns in the dataset:

- **`neo_id`**: Unique identifier for each near-Earth object.
- **`name`**: Name of the near-Earth object.
- **`absolute_magnitude`**: The absolute magnitude of the NEO, indicating its brightness.
- **`estimated_diameter_min`**: Minimum estimated diameter of the NEO (in kilometers).
- **`estimated_diameter_max`**: Maximum estimated diameter of the NEO (in kilometers).
- **`orbiting_body`**: The primary celestial body that the object is orbiting.
- **`relative_velocity`**: Velocity of the NEO relative to Earth (in kilometers per hour).
- **`miss_distance`**: The distance at which the object will miss Earth (in kilometers).
- **`is_hazardous`**: Indicates whether the NEO is classified as hazardous.

## **Data Cleaning and Preprocessing**

The dataset underwent multiple cleaning and preprocessing steps to prepare it for analysis and modeling:

- **Handling Missing Values**: Missing values in columns such as `absolute_magnitude`, `estimated_diameter_min`, and `estimated_diameter_max` were imputed with the mean values of their respective columns.
- **Outlier Treatment**: Outliers were detected and replaced with mean values to reduce their impact on model performance.
- **Feature Engineering**: New columns for the year and object code were extracted from the `name` column to provide additional insights for analysis.
- **Label Encoding**: Categorical variables such as `orbiting_body` and `is_hazardous` were label-encoded using `LabelEncoder` for model training.

## **Data Analysis and Visualizations**

Several analytical questions were explored to better understand the dataset and identify trends:

- **Distribution Analysis**: Examined the distribution and statistics for key features like `absolute_magnitude`, `estimated_diameter_min`, `estimated_diameter_max`, and `relative_velocity`.
- **Hazard Trends**: Analyzed the trend of hazardous objects over the years and across different orbiting bodies.
- **Size and Hazard Relationships**: Investigated the relationship between the size of an object and its hazard classification.

Visualizations such as histograms, box plots, and pie charts were created to provide insights into data distribution, outliers, and trends.

## **Modeling and Evaluation**

A **Random Forest Classifier** was used to build a predictive model that determines whether a near-Earth object is hazardous. Below are the steps taken:

1. **Train-Test Split**: The dataset was split into training (80%) and testing (20%) sets.
2. **Model Training**: The Random Forest model was trained on the training data.
3. **Model Evaluation**: The model's accuracy was assessed on both the training and testing sets to ensure robust performance.
4. **Performance Metrics**: Key metrics such as precision, recall, F1-score, and accuracy were calculated using a classification report.

### **Model Performance**

- **Training Accuracy**: The model achieved a high accuracy on the training set, indicating it was able to capture the patterns in the data effectively.
- **Test Accuracy**: The model also performed well on unseen data, showcasing good generalization ability.
- **Classification Report**: Precision, recall, and F1-score were computed to evaluate the model’s performance on the test set.

## **Conclusion**

This project successfully analyzed and modeled the Near-Earth Objects dataset to predict which objects could be hazardous. Through careful data cleaning, visualization, and modeling, we were able to gain valuable insights into the nature of NEOs and develop a robust classification model.
"""

