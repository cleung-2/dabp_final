# Improving Maternal and Child Health in Pennsylvania

This is the repository for all datasets and Jupyter notebooks utilized in our project. The goal of the project is to provide an allocation prioritization for each county in Pennslyvania for four areas of interest related to improving maternal, infant, and child health (MICH) outcomes. The repository contains the datasets and notebooks used at every stage of our process. The key files to run that provided the main results of our project are in the main folder and explained in the 'Main Files' section below. Data preprocessing steps, raw data sources, and other exploratory notebooks are also stored within other folders in our repository.

*To check the results of our project, the main notebook to examine is the 'OptimizationCode.ipynb'. How all other notebooks and files are connected are explained below. *

## Main Files
**OptimizationCode.ipynb**

This notebook contains the optimization implementation of our project. The purpose of the notebook is to determine the prioritization allocation of the programs that were determined from our linear regression model. It references the 'parameters.csv' and 'regression_results.csv'. The final results of our project are contained in this notebook.

**LinearRegression.ipynb**

This notebook contains our linear regression modeling of our project. The purpose of the notebook is to find what are the most important variables that contribute to achieving MICH goals across the state of Pennslyvania and to obtain coefficient weights to use in our optimization formulation. The notebook contains the entire modeling training and evaluation process. The 'parameters.csv' and 'regression_results.csv' come from this notebook. Please note that these two lines have been commented out because a seed was not intially set with the results that the final optmization results used.

**parameters.csv**

This csv file contains the county values that are used in our optimization problem. It comes from 'LinearRegression.ipynb'.

**regression_results.csv**
This csv file contains the coefficient weights that were found from our linear regression model in 'LinearRegression.ipynb'.

## Preprocessing and EDA folder
This folder contains all the notebooks used to clean and preprocess the data used in our future modeling. It also contains some EDA.

## Data folder
This folder contains the raw and cleaned datasets, in csv form, that were utilized in the project. These datasets are used in the preprocessing and linear regression stages of our project. 

## Old Exploratory folder
This folder contains some other model types, such as CART and classifiers, that were tested in early iterations of the project. These files have no impact on the actual findings of our project.
