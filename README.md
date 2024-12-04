# Analysis of Drug-Target Interactions Using Machine Learning

This work is developed in the ambit of the curricular unit *Intelligent Systems for Bioinformatics* of the Bioinformatics Master's program by:

- Sofia Ferreira
- Laís Carvalho
- Armindo Machado
- Afonso Sá


This project involves the analysis of the DAVIS dataset using machine learning techniques, leveraging Python as the programming language. 
The work is documented in a Jupyter Notebook, structured into logical sections that outline each step of the analysis. 

# Project Description
The goal of this project is to analyze the Drug-Target Interactions (DTI) present in the [DAVIS dataset](https://tdcommons.ai/multi_pred_tasks/dti), which focuses on the interaction of kinase inhibitors with human kinases. 
This dataset provides an opportunity to design predictive models that can estimate binding affinities between drugs and protein targets. 
The primary aim is to create a machine learning model capable of predicting these affinities, thereby contributing to advancements in drug discovery and precision medicine.

## About the Dataset
The DAVIS dataset contains detailed information about:
- 72 kinase inhibitors interacting with 442 kinases, covering over 80% of the human catalytic protein kinome;
- Task: Regression. Predict the binding affinity between drug compounds (represented as SMILES strings) and target proteins (represented as amino acid sequences);
- Statistics: 25,772 drug-target interaction (DTI) pairs, 68 drugs, and 379 proteins;
- Splits: Random Split, Cold Drug Split, Cold Protein Split.

# Dataset Access
To access the dataset and prepare it for analysis, the following code can be used:

```python
from tdc.multi_pred import DTI
data = DTI(name='DAVIS')
split = data.get_split()
```

# Project Workflow
This project is divided into the following sections:

1. Data Exploration and Preprocessing
Objective: Understand the structure and characteristics of the dataset.
Perform exploratory data analysis to visualize and summarize key patterns and distributions.
Preprocess the dataset by handling missing values, generating features, and normalizing data as needed.

2. Dimensionality Reduction and Clustering
Utilize unsupervised learning techniques to visualize high-dimensional data.
Apply clustering methods to identify inherent patterns in the data.

3. Machine Learning Models
Compare the performance of multiple machine learning models using appropriate metrics.
Optimize hyperparameters to improve predictive accuracy.
Select the best-performing model for the dataset.

4. Deep Learning Models
Develop and train deep learning models to predict drug-target binding affinities.
Evaluate the performance of these models and analyze their results critically.
