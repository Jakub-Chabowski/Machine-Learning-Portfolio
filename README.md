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
### Current Notebooks
#### Analysis.ipynb
Contains the data audit as well as results of normalising the target using different methods
#### Preprocessing & Baseline.ipynb
Includes the initial preprocessing decisions as well as a variety of tests around deciding a baseline model

To run the notebook: click Run in the header, then select Restart Kernel and Run All