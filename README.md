# Glyphnet

*Glyphnet* is a repository that includes an example of a deep learning approach to ancient Egyptian hieroglyphs classification, ...

If you use this repository, please cite it as:

A. Barucci, C. Cucci, M. Franci, M. Loschiavo and F. Argenti, **A Deep Learning Approach to Ancient Egyptian Hieroglyphs Classification**. IEEE Access, vol. 9, pp. 123438-123447, 2021, doi: 10.1109/ACCESS.2021.3110082.

This document provides a quick introduction to the SCRIPT NAME HERE to help new users get started.  

Please read the [LICENSE.md](./LICENSE.md) file before using *Glyphnet*.

## Requirements (TO DO)

Open a terminal window (for Unix users) or Anaconda Prompt (for Windows users), activate or create a Python environment with Python version 3.9.1 installed (we recommend to create a new Python environment, see below) and install the following Python packages (if packages already exist, check the version)

```
pip install mlxtend==0.18.0
pip install matplotlib==3.3.3
pip install pandas==1.2.0
pip install numpy==1.19.5
pip install openpyxl==3.0.5
pip install scikit-learn==0.24.0
```


### Create a new local Python virtual environment using conda: (TO DO)
1. Create a new folder with the name of your new environment (e.g., Schizo_env)
2. Open a terminal window (for Unix users) or Anaconda Prompt (for Windows users), from the folder that contains Schizo_env directory and type:

```
conda create --prefix ./Schizo_env
```

```
conda activate ./Schizo_env
```

```
conda install python=3.9.1
```


## Usage (TO DO)

```
python Schizotypy_group_prediction.py --help

Usage: Schizotypy_group_prediction.py [-h] XLSX_file

A machine learning predicitive model, optimized in a nested stratified cross-validation loop repeated 1000 times

positional arguments:
  XLSX_file   XLSX file including data

optional arguments:
  -h, --help  show this help message and exit
```

## Testing (TO DO)

## Ouputs (TO DO)
The outputs are stored in two different folders: *Figures* contains the ROC curve plot and *csv\_results* includes all the csv files. Specifically:

* *CombsSelected.csv* reports the number of times each feature combination has been selected
* *Scores.csv* includes average and standard deviation values of balanced accuracy, area under the ROC curve, sensitivity and specificty obtained both in the training and test sets
* *tpr.csv* reports average true positive rate values (among repetitions and nested CV splits)

## Authors
* **Andrea Barucci** - *Researcher at at Institute of Applied Physics "Nello Carrara" (IFAC) – National Council of Research (CNR), Sesto Fiorentino, Italy.* Email address: <a.barucci@ifac.cnr.it>

