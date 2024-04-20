# Parameter_Optimization_102117024
# Optimizing SVM Performance on Pen-Based Recognition of Handwritten Digits

This study showcases advanced techniques to boost the efficiency of Support Vector Machine (SVM) applied to the Pen-Based Recognition of Handwritten Digits data sourced from the UCI Machine Learning Repository. This data set encompasses samples from 44 writers. These writers are asked to write digits in random order inside boxes of 500 by 500 tablet pixel resolution. 

## Data Overview

The Pen-Based Recognition of Handwritten Digits encompasses 7,494 records, each with 16 attributes. The dataset is segmented into ten separate subsets for both training and validation purposes.

**Dataset Link:** https://archive.ics.uci.edu/dataset/81/pen+based+recognition+of+handwritten+digits

## Approach

1. **Data Ingestion**: We employ the pandas library to ingest the data from a CSV file.

2. **Data Partitioning**: The data is bifurcated into training and validation subsets at a 70-30 ratio, and this process is reiterated tenfold to create ten varied samples.

3. **Optimizing SVM**: For each sample, SVM is fine-tuned using cross-validation involving 100 cycles. We utilize GridSearchCV to pinpoint the most effective hyperparameters.

4. **Performance Metrics**: We capture the optimal parameters and associated accuracy levels for each sample. We then pinpoint the sample with the highest accuracy.

  ![image](https://github.com/joyy2002/Parameter_Optimization_102117024/assets/102287699/c44a9120-3bcf-4c13-a228-dca0681631d4)

5. **Performance Visualization**: A visualization is crafted for the top-performing sample, showcasing the fluctuation in training and validation accuracies across the optimization iterations.
![image](https://github.com/joyy2002/Parameter_Optimization_102117024/assets/102287699/b7e0bac7-b02a-4de8-917a-896e231bafdc)

 


## Included Assets

- `dataset.csv`: The main CSV file containing the Pen-Based Recognition of Handwritten Digits dataset.
- `parameter_optimization_102117024.ipynb`: Jupyter Notebook housing the Python scripts for the study.
- `README.md`: This document, offering insights into the project.

## System Requirements

- Python 3.x
- Essential libraries: numpy,pandas, scikit-learn, matplotlib


