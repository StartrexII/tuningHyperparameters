# <center> Hyperparameter selection methods

## Table of contents
1. [Project Description](#Project-Description)
2. [Data description](#Data-description)
3. [Libraries](#Libraries)
4. [Project Installation](#Project-Installation)
5. [Using the project](#Using)
6. [Authors](#Authors)

## Project Description

The objective of the competition is to help us build as good a model as possible so that we can, as optimally as this data allows,
relate molecular information, to an actual biological response.

**Problem** - to build a classifier that determines biological activity.

**This project** aims to optimize the hyperparameters of two popular classification models in various ways and includes:

* loading and splitting data into samples([the data has been prepared](#Data-description))
* building a logistic regression and a random forest based on default parameters
* tuning of hyperparameters using [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html 'scikit-learn.org')
* tuning of hyperparameters using [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html 'scikit-learn.org')
* tuning of hyperparameters using [Hyperopt](https://hyperopt.github.io/hyperopt/)
* tuning of hyperparameters using [Optuna](https://optuna.org 'optuna.org')
* analysis of results

**Project structure:**
* [data](./data) - the folder with the original tabular data
* [plotly](./plotly) - a folder with charts for viewing them in the browser
* [predictingTheBiologicalResponse.ipynb](./predictingTheBiologicalResponse.ipynb) - jupyter-notebook containing the main project code
* [requirements.txt](./requirements.txt) - a file with the versions of the modules used, for reproducibility of the code

:arrow_up:[To the table of contents](#table-of-contents)

## Data description

 We have shared the data in the comma separated values (CSV) format. Each row in this data set represents a molecule. The first column contains experimental data describing an actual biological response; the molecule was seen to elicit this response (1), or not (0). The remaining columns represent molecular descriptors (d1 through d1776), these are calculated properties that can capture some of the characteristics of the molecule - for example size, shape, or elemental constitution. The descriptor matrix has been normalized. 

:arrow_up:[To the table of contents](#table-of-contents)

## Libraries

* Python (3.11.1):
    * [pandas (2.0.1)](https://pandas.pydata.org)
    * [numpy (1.24.3)](https://numpy.org)
    * [seaborn (0.12.2)](https://seaborn.pydata.org)
    * [scikit-learn (1.2.2)](https://scikit-learn.org/stable/)
    * [hyperopt (0.2.7)](https://hyperopt.github.io/hyperopt/)
    * [optuna (3.2.0)](https://optuna.readthedocs.io/en/stable/index.html)

:arrow_up:[To the table of contents](#table-of-contents)

## Project Installation

```
    git clone https://github.com/StartrexII/tuningHyperparameters
```

:arrow_up:[To the table of contents](#table-of-contents)                        

## Using

All other information is presented in the jupyter-notebook [predictingTheBiologicalResponse.ipynb](./predictingTheBiologicalResponse.ipynb).
If the graphs are not displayed on GitHub, you can open them in the browser, they are in the folder [`plotly/`](./plotly)

:arrow_up:[To the table of contents](#table-of-contents)

## Authors

* [Егор Орлов](https://vk.com/liquidlogic)

:arrow_up:[To the table of contents](#table-of-contents)

If the information on this project seems interesting or useful to you, then I will be very grateful to you if you mark the repository and profile with ⭐️⭐️⭐️:)