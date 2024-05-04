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

## Poster

The poster titled "The Benefits of College Athletic Success: An Application of the Propensity Score Design" is detailed in the file `ML_PSM.pdf`. It encapsulates the essence of our project, which is to apply machine learning techniques to enhance the understanding and outcomes of college athletic success on institutional health metrics such as alumni donations. The poster includes:

- An abstract that outlines the objectives and the scope of our analysis.
- A detailed introduction that sets the stage for the methodology applied and the reasons behind it.
- A literature review that supports the use of Random Forest regression and Logistic Regression in our study.
- A comprehensive methodology section that describes how we implemented machine learning techniques to refine the analysis.
- Findings that summarize the impact of athletic success on alumni donation behaviors, comparing results obtained through traditional Propensity Score Matching (PSM) and advanced machine learning (ML) techniques.
- A discussion that interprets the results in the context of existing literature and their implications for the broader field of educational economics and fundraising.

This poster serves as a visual and textual representation of our work, providing insights into the intricate relationship between collegiate sports success and its broader institutional impacts. It's ideal for stakeholders interested in the analytical techniques and outcomes of this study.

You can view and download the poster directly from the repository: [ML_PSM.pdf](./ML_PSM.pdf).
You can view and download the Overleaf from this link: [Overlead Link](https://www.overleaf.com/project/6627ce5f5923f9a7550467d9).

## Supplemental Document
The supplemental document includes a comprehensive literature review supporting the analytical techniques used in our study and presents various graphs illustrating key aspects of our findings. This document provides deeper insights into the theoretical framework and empirical analysis underpinning our research. Access the supplemental document here:

[Supplemental Literature Review and Graphs](https://docs.google.com/document/d/1t6xMcOxghhCqV8nGC4FjSOGPpSo3UFj6wVu9TVDwQFo/edit?usp=sharing)


### `Report`
*Coming soon* - This document will provide a comprehensive report on the methodology, analysis, and results of the project.

## How to Use
To use the code, you can either download the Python files and CSV to run the scripts locally, or you can click on the links below to access the scripts in Google Colab, where they can be run directly in your browser without any setup (if running ML Extension you have to run the sections in order or th efile won't run (if you run a section twice you have to start over to ensure proper column allignment):

- [PSM ML Extension in Colab](https://colab.research.google.com/drive/1D9Wbt3Y0g8Q_cBkghSxpT-2ObatIjY4r#scrollTo=LMo4D9LT-bwZ)
- [PSM Replication in Colab](https://colab.research.google.com/drive/1u4YxK_ndsvyyUrCngM23oq6DXMdRFQhu#scrollTo=P4ikY0mY8PEY)

## Original Study and Data Source

### Original Paper
The project is a replication and extension of the study published in [The Review of Economics and Statistics](https://direct.mit.edu/rest/article-abstract/99/1/119/58365/The-Benefits-of-College-Athletic-Success-An?redirectedFrom=fulltext), titled "The Benefits of College Athletic Success: An Application of the Propensity Score Design". We encourage users to refer to the original paper for a comprehensive understanding of the research context and methodology.

### Data Source
The dataset used for this project is available on [Harvard's Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/ASXOBS). This repository contains all the data required to replicate the analyses presented in the original study. Users looking to replicate or extend the analysis are recommended to download the data directly from this source.

## Contributors

We thank all contributors who have worked on this project. Feel free to connect with them or reach out for more information:

- [Ty McClure](https://www.linkedin.com/in/ty-mcclure-b65391236)
- [Natalie Mikosz](https://www.linkedin.com/in/natalie-mikosz-880b79250/)
- [Anshu Puppala](https://www.linkedin.com/in/anshuman-puppala-73274226a/)
- [Ethan Tabtiang](https://www.linkedin.com/in/ethan-tabtiang-b8a017127/)
- [Juan Rodriguez](https://www.linkedin.com/in/juan-rodriguez-3a1228294/)



