# PSM Machine Learning Replication

## Introduction
* For this repo we will be working to replicate "The Beneﬁts of College Athletic Success: An Application of the Propensity Score Design" and then work to apply new Machine Learning techniques to improve upon the paper's model.

## Files Description

### `Formatted_data.csv`
This CSV file contains all the data necessary for replication. It was created by merging two smaller CSV files and is referenced in both of the scripts provided in this repository.

### `PSM_ML_extension.py`
This script applies machine learning techniques to improve the analysis of a dataset derived from sports and academic performance metrics. The script performs the following operations:
- Loads and preprocesses data from `Formatted_data.csv`, selecting necessary columns and creating lagged variables.
- Implements feature scaling and imputation to handle missing values.
- Calculates propensity scores using logistic regression and random forest classifiers.
- Conducts matching using nearest neighbors to find control groups for treated samples.
- Evaluates the model's performance through confusion matrices and classification reports.
- Uses Elastic Net to estimate regression models and a random forest regressor to analyze feature importance and prediction errors.

### `PSM_Replication.py`
This script replicates a paper's methodology, extending it with additional regression analysis. It performs the following tasks:
- Loads data from `Formatted_data.csv` and processes it to ensure it is ready for analysis.
- Identifies and selects variables of interest, especially lagged ones, for analysis.
- Conducts regression analysis using Ordinary Least Squares (OLS) and Instrumental Variable (IV) methods.
- Implements robust error handling and data filtering to manage missing data and ensure data integrity.
- Outputs analysis results including summary statistics and graphs.

### `Poster`
*Coming soon* - This file will contain the poster that summarizes the project and its findings.

### `Report`
*Coming soon* - This document will provide a comprehensive report on the methodology, analysis, and results of the project.

## How to Use
To use the code one would have to download the python files as well as the csv to run the scripts. There are multiple different libraries that may need to be downlaoded but beyond that the code will run without user oversight. 

## Original Study and Data Source

### Original Paper
The project is a replication and extension of the study published in [The Review of Economics and Statistics](https://direct.mit.edu/rest/article-abstract/99/1/119/58365/The-Benefits-of-College-Athletic-Success-An?redirectedFrom=fulltext), titled "The Benefits of College Athletic Success: An Application of the Propensity Score Design". We encourage users to refer to the original paper for a comprehensive understanding of the research context and methodology.

### Data Source
The dataset used for this project is available on [Harvard's Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/ASXOBS). This repository contains all the data required to replicate the analyses presented in the original study. Users looking to replicate or extend the analysis are recommended to download the data directly from this source.

## Contributors

We thank all contributors who have worked on this project. Feel free to connect with them or reach out for more information:

- [Ty McClure](https://www.linkedin.com/in/ty-mcclure-b65391236)
- [Natalie Mikosz](https://www.linkedin.com/in/natalie-mikosz-880b79250/)
- [Ethan Tabtiang](https://www.linkedin.com/in/ethan-tabtiang-b8a017127/)
- [Anshu Puppala](https://www.linkedin.com/in/anshuman-puppala-73274226a/)
- Juan Rodriguez - Email: [juantico@tamu.edu](mailto:juantico@tamu.edu)



