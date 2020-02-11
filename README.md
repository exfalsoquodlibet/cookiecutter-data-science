# Cookiecutter Data Science GDS

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._


#### [Project homepage](http://ukgovdatascience.github.io/cookiecutter-data-science-gds/)


### Acknowledgment:
-----------
This project builds on 
[drivendata's cookiecutter-data-science project template](http://drivendata.github.io/cookiecutter-data-science/) 
#cookiecutterdatascience


### Requirements to use the cookiecutter template:
-----------
 - Python 3.6 or above
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be 
 installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/ukgovdatascience/cookiecutter-data-science-gds




### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
    ├── .envrc                        <- Where to declare individual user environment variables
    ├── .flake8                       <- Flake8 linting configuration file used in the GDS Way
    ├── .gitignore                    <- Files and directories to be ignored by git
    ├── .secrets                      <- (optional) Where to store credentials - this will not be tracked by Git
    ├── CONTRIBUTING.md               <- Guide to how potential contributors can help with your project
    ├── LICENSE
    ├── Makefile                      <- Makefile with commands like `make data` or `make train`
    ├── README.md                     <- The top-level README for developers using this project.
    ├── requirements.txt              <- The requirements file for reproducing the analysis environment, e.g.
    │                                    generated with `pip freeze > requirements.txt`
    ├── setup.py                      <- makes project pip installable (pip install -e .) so src can be imported
    ├── test_environment.py           <- Python environment tester   
    │
    ├── data
    │   ├── external                  <- Data from third party sources.
    │   ├── interim                   <- Intermediate data that has been transformed.
    │   ├── processed                 <- The final, canonical data sets for modeling.
    │   └── raw                       <- The original, immutable data dump.
    │
    ├── docs                          <- A default Sphinx project; see sphinx-doc.org for details
    │   ├── aqa_plan.md               <- AQA plan for the project
    │   └── assumptions_log.md        <- where to log key assumptions to data / models / analyses
    │   └── pull_request_template.md  <- Pull request template
    │
    ├── models                        <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks                     <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                                    the creator's initials, and a short `-` delimited description, e.g.
    │                                    `1.0-jqp-initial-data-exploration`.
    │
    ├── reports                       <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures                   <- Generated graphics and figures to be used in reporting
    │
    └── src                           <- Source code for use in this project.
        ├── make_data                 <- Scripts to download or generate data
        ├── make_features             <- Scripts to turn raw data into features for modeling
        ├── make_models               <- Scripts to train models and then use trained models to make predictions
        ├── make_visualisations       <- Scripts to create exploratory and results oriented visualizations
        └── tools                     <- Any helper scripts go here

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">
cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

```


### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
