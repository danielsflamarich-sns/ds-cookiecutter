datascience-cookiecutter
==============================

Template for Data Science projects


Requirements
------------

Python >= 3.5

[cookiecutter Python package](https://pypi.org/project/cookiecutter/) >= 1.4.0: `pip install cookiecutter`


Starting a new project
------------

Run this command line, answer a few questions, and cookiecutter will automatically create the directory.

`cookiecutter https://github.com/danielsflamarich-sns/ds-cookiecutter.git`

After that, go to the newly created folder and create a new environment (in this case, the environment name is `env`):

`python3 -m venv env`

Activate newly created environment:

`source env/bin/activate`

And lastly, install Sonosuite's data team python package:

`pip install git+https://github.com/danielsflamarich-sns/dataanalytics-sns-python-package`


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for data scientists using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── processed      <- The final data. Clean/engineered/canonical data sets for modeling
    │   ├── queries        <- SQL statements for connections.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number with a zero on the left (for ordering),
    │                         the creator's initials, underscore plus delimited description, e.g.
    │                         `01_dsf_exploratory_data_analysis`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── plots          <- Generated graphics/plots/figures to be used in reporting/slides
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    ├── utils              <- Python functions used in the notebooks
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project
    │   ├── __init__.py    <- Makes src a Python module
    │   ├── connections    <- Redshift connections
    │   ├── data           <- Scripts to download/generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------
