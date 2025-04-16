# Heart Disease Analysis & Prediction

This project is dedicated to analyze the heart disease dataset and developing predictive models using machine learning. It leverages various datasets along with preprocessing and visualization techniques, primarily using Python libraries.

## Project Structure

- **heart_disease.ipynb**  
  Main Jupyter Notebook with exploratory data analysis, preprocessing steps, and model setup.
- **processed.cleveland.data**  
  Processed heart disease dataset.
- **README.md**  
  This file.

## Prerequisites & Libraries

Before running the notebook or scripts, ensure you have the following libraries installed:

- **Python 3.7+**
- **Jupyter Notebook** or **Jupyter Lab**
- **pandas** – for data manipulation and analysis (`pip install pandas`)
- **numpy** – for numerical computations (`pip install numpy`)
- **scikit-learn** – for machine learning algorithms and preprocessing (`pip install scikit-learn`)
- **matplotlib** / **seaborn** – for data visualization (`pip install matplotlib seaborn`)

Additional libraries may be required depending on your analysis needs. Check the notebook for any additional dependencies.

## Methodology and Models

- The dataset was checked for errors, missing data, and overall correctness. Missing data was imputed using a SimpleImputer with the most frequent value for each column.

- Data was preprocessed using a StandardScaler and then split into three groups for training, validation, and testing. The split was 70% for training/validation (with a further split of 80% for training and 20% for validation) and 30% for testing.
  
- Multiple models were used to identify the best predictors of heart disease, focusing on recall as the primary metric. Logistic Regression and AdaBoost achieved the best results.

- The final AdaBoost model achieved accuracy, recall, precision, and F1 scores of 0.91.