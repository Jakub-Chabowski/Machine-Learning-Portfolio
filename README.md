# CT 4101 Machine-Learning-Portfolio

## Dataset

### Name: 
Forest Fires
### Source: 
UC Irvine https://archive.ics.uci.edu/dataset/162/forest+fires
### Licence: 
Creative Commons Attribution 4.0 International
### Citation: 
P. Cortez and A. Morais. "Forest Fires," UCI Machine Learning Repository, 2007. [Online]. Available: https://doi.org/10.24432/C5D88D.

# Setup:
Ran using Python 3.12.3

### Create Virtual Environment
    python -m venv .venv

### Activate virtual environment 

#### macOS / Linux
    source .venv/bin/activate

#### Windows PowerShell
    .venv\Scripts\Activate.ps1

### Install required packages
    python -m pip install -r requirements.txt

## Data
Download data from https://archive.ics.uci.edu/dataset/162/forest+fires

Place unzipped data into the data/ directory so that the path is as follows:
data/forest+fires/forestfires.csv

# Run
    jupyter lab
Open the notebooks directory and open the notebook you want to run
## Current Notebooks

### Conclusions.ipynb
Contains conclusions derived from the evidence and findings produced by the notebooks in /_MAIN/
Right now, contains the Milestone 3 Conclusions and future plans

### /_MAIN
#### These notebooks contain the main summaries of findings and allow for the evidence that these findings are based on the be collated
#### /Hyperparameters_and_data.ipynb
Contains code to read in data and stores any global hyperparameters (currently only RANDOM_STATE)
#### /Run_all_analysis.ipynb
Includes findings and runs all of the relevant analysis notebooks
#### /Run_all_models_and_findings.ipynb
Includes findings and runs all of the models

### /Analysis
#### /Analysis.ipynb
Contains the data audit as well as results of normalising the target using different methods. As well as this prints out the effects that the different pre-processing pipelines having on the dataset
#### /Feature_Importance.ipynb
Uses a RandomForestRegressor to extract feature importances using MDI and prints assoicated graphs

### /Models
#### /Train_Test_Split.ipynb
Runs the models and preprocessing pipelines using a train_test_split and outputs graphs for Residual Analysis, MAE, RMSE, and R2 Score
#### /Neural_Networks.ipynb
Runs a limited number of MLPRegression models and compares them to the Baseline Model and outputs graphs for Residual Analysis, MAE, RMSE, and R2 Score
#### /Cross_Validate.ipynb
Runs the models and preprocessing pipelines using RepeatedKFold cross_validation and outputs graphs for MAE, RMSE and R2 Score

### /Preprocessing
#### /Preprocessing.ipynb
Includes the defintions for all of the pre-processing pipelines as well as the models that are used. These are accessed by the other notebooks.

To run the notebook: click Run in the header, then select Restart Kernel and Run All