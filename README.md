# Heart-Attack-Prediction
Heart disease, particularly heart attacks, is one of the leading causes of death globally. Our objective is to develop a predictive model that identifies individuals at risk based on demographic, lifestyle, and medical factors. The results are then visualized in Power BI for easy interpretation and actionable insight.

# Table of Contents
- Project Overview
- Dataset
- Technologies Used
- Algorithm
- Power BI

# Project Overview
This project focuses on predicting heart attacks using a dataset from Kaggle. To make predictions, a Machine Learning model was created using the Decision Tree algorithm. The model is then exported into Power BI to show the prediction on the data. The Power BI project shows relationships of different features from the dataset and how it affects the final prediction using graphs and figures.     

# Dataset
A dataset is an essential requirement for creating a Machine Learning model. This project focused mainly on "Heart Deases" datasets. The size of the used dataset is ~250,000 records, with features such as: Age, Sex, Income, Smoking, Alcohol, and so on.
The first step is to prepare the dataset for creating an ML model. The preprocessing step includes: delete null values, convert all categorical data into numerics, and columns with high variation should be changed into categories (and then to numerics). After the preprocessing step, use algorithms to find which features have the highest impact on the target column (we used a heatmap).
Finally, load the dataset into Power BI.    
      
The dataset was found on Kaggle:https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease. 

# Technologies Used
- Power BI for interactive dashboards
- Python (Scikit-learn) for implementing the Decision Tree model
- Pandas, NumPy, Matplotlib for data preprocessing and visualization
- Jupyter Notebook (for testing ML logic)
- Power Query for data transformation inside Power BI

# Algorithm
There are many algorithms that can be used for designing a Machine Learning model. To predict the likelihood of heart disease, we implemented a Decision Tree Classifier using the ID3 algorithm (Information Gain as the splitting criterion). This model was chosen for its interpretability and ability to handle both categorical and numerical features without requiring normalization. 
Refer to "Heart Attack ML Model.py" file for a detailed explanation of how to create a ML model.   
 
# Power BI
For representation of the results and relationships of features and the final target, we used Power BI. 

Step 1: Load the dataset into Power BI and preprocess. 
- Click "Transform Data" to open Power Query Editor
- Perform the following:
- Rename columns for clarity (if needed)
- Encode categorical variables using "Replace Values" or "Conditional Columns"
- Create new columns for categorized features (e.g., group BMI or SleepTime into categories)
- Remove duplicates or unnecessary columns
- Click "Close & Apply"   

Step 2: Create Relationships (in case you use multiple datasets)
- Go to "Model" view
- Drag and drop to link related columns (e.g., ID between tables if applicable)
- Ensure 1-to-many relationships are correctly defined

Step 3: Add Machine Learning Model
- Click on the Python visual icon in the Visualizations pane
- Add necessary fields (e.g., Age, BMI, etc.)
- Paste your trained model code (from Heart Attack ML Model.py)
- Make sure Python is installed and configured:
- Use File > Options > Python scripting to set Python environment

Step 4: Add Visualizations
1. Use the Visualizations pane to insert visuals:
      - Pie Chart – for class distribution
      - Stacked Column Chart – for comparing feature categories vs. risk
      - Filled Map – for geographic analysis
      - Slicer – to filter by gender, age, etc.
      - Scatter/Area Chart – for trends and patterns
2. Drag relevant fields into the "Values", "Axis", or "Legend" areas

Collaborators:
1. Begimai Alisherova - begima.a.13@gmail.com 
2. Raiyan Mokhammad - raiyan.mokhd@gmail.com 
