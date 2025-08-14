# K-Nearest Neighbors (KNN) Classification on Iris Dataset

## Project Overview
This project applies the K-Nearest Neighbors (KNN) classification algorithm to the well-known Iris dataset.  
The Iris dataset contains measurements of iris flowers from three species: **setosa**, **versicolor**, and **virginica**.  
The goal is to train a model that can correctly predict the species of an iris flower based on four features:
- Sepal length
- Sepal width
- Petal length
- Petal width

## What I Did
1. **Data Loading and Preprocessing**  
   - Loaded the Iris dataset from scikit-learn’s built-in datasets.  
   - Split the dataset into training (70%) and testing (30%) sets.  
   - Standardized the feature values so that all measurements have the same scale.  

2. **Model Training**  
   - Trained the KNN algorithm with different values of **K** (1, 3, 5, 7, 9) to find the best number of neighbors.  
   - Measured the accuracy for each K value on the test set.  

3. **Model Evaluation**  
   - Chose **K = 5** as the best option (although K = 3, 5, 7, and 9 all achieved the same best accuracy).  
   - Evaluated the model performance using:
     - **Confusion Matrix** to see correct and incorrect predictions for each class.
     - **Classification Report** to get precision, recall, and F1-score for each species.

## What I Got (Results)
- **Accuracy Scores for Different K Values**  
  - K = 1 → 97.78%  
  - K = 3 → 100%  
  - K = 5 → 100%  
  - K = 7 → 100%  
  - K = 9 → 100%  

- **Best Accuracy Achieved:** 100%  
- **Confusion Matrix:** Perfect classification (no misclassifications).  
- **Classification Report:**  
  - Precision = 1.00 for all species  
  - Recall = 1.00 for all species  
  - F1-score = 1.00 for all species  

## Conclusion
The KNN algorithm performed exceptionally well on the Iris dataset, achieving perfect accuracy with multiple values of K.  
This is likely due to the dataset being well-separated and relatively small.  
For real-world datasets with more noise and overlapping classes, performance may not be this high, and careful tuning of K along with proper validation would be required.

## How to Use
- Open the notebook in Jupyter Notebook or JupyterLab.  
- Run all cells in order.  
- The notebook will print accuracy scores for different K values and show evaluation metrics for the best model.
