# Cookiecutter Data Science GDS

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._

#### [Project homepage](http://ukgovdatascience.github.io/cookiecutter-data-science-gds/)

### Acknowledgment:

This project builds on 
[drivendata's cookiecutter-data-science project template](http://drivendata.github.io/cookiecutter-data-science/) 
#cookiecutterdatascience

### Requirements to use the cookiecutter template:

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

    cookiecutter https://github.com/ukgovdatascience/cookiecutter-data-science-gds

Then make sure to complete the relevant Analytical Quality Assurance (AQA) documents - instructions can be found 
[here]({{%20cookiecutter.repo_name%20}}/docs/README.md#getting-started).

### The resulting directory structure

The directory structure of your new project looks like this: 

```
    ├── .envrc                          <- Where to declare individual user environment variables
    ├── .flake8                         <- Flake8 linting configuration file used in the GDS Way
    ├── .gitignore                      <- Files and directories to be ignored by git
    ├── .secrets                        <- (optional) Where to store credentials - this will not be tracked by Git
    ├── CONTRIBUTING.md                 <- Guide to how potential contributors can help with your project
    ├── LICENSE
    ├── Makefile                        <- Makefile with commands like `make data` or `make train`
    ├── README.md                       <- The top-level README for developers using this project.
    ├── requirements.txt                <- The requirements file for reproducing the analysis environment, e.g.
    │                                      generated with `pip freeze > requirements.txt`
    ├── setup.py                        <- makes project pip installable (pip install -e .) so src can be imported
    ├── test_environment.py             <- Python environment tester   
    │
    ├── data
    │   ├── external                    <- Data from third party sources.
    │   │
    │   ├── interim                     <- Intermediate data that has been transformed.
    │   │
    │   ├── processed                   <- The final, canonical data sets for modeling.
    │   │
    │   └── raw                         <- The original, immutable data dump.
    │
    ├── docs                            <- A default Sphinx project; see sphinx-doc.org for details    
    │   ├── conf.py                     <- Sphinx configuration file
    │   ├── index.md                    <- main Markdown page for the Sphinx documentation
    │   ├── make.bat                    <- command file for Sphinx documentation
    │   ├── Makefile                    <- Makefile for Sphinx documentation
    │   ├── pull_request_template.md    <- Pull request template
    │   ├── README.md                   <- README detailed how to view/build the Sphinx documentation
    │   │
    │   ├── _static                     <- folder containing static files used by the Sphinx documentation
    │   │
    │   ├── aqa                         <- folder for Analytical Quality Assurance (AQA) documentation
    │   │   ├── aqa_plan.md             <- AQA plan overview for the project
    │   │   ├── assumptions_log.md      <- where to log key assumptions to data / models / analyses
    │   │   ├── build.md                <- AQA plan for the build stage of the project
    │   │   ├── design.md               <- AQA plan for the design stage of the project
    │   │   ├── general.md              <- AQA plan for the general stage of the project
    │   │   ├── README.md               <- main Markdown page for the `docs/aqa` folder
    │   │   └── release.md              <- AQA plan for the release stage of the project
    │   │
    │   ├── getting_started
    │   │   └── README.md               <- main Markdown page for the `docs/getting_started` folder; contains general 
    │   │                                  instructions for getting started with this project
    │   │
    │   └── reference                   <- folder for documentation of `src`-specific functions
    │       ├── make_data.md            <- documentation for `src.make_data` functions
    │       ├── make_features.md        <- documentation for `src.make_features` functions
    │       ├── make_models.md          <- documentation for `src.make_models` functions
    │       ├── make_visualisations.md  <- documentation for `src.make_visualisations` functions
    │       ├── README.md               <- main Markdown page for the `docs/reference` folder
    │       ├── src.md                  <- documentation for `src` functions
    │       └── tools.md                <- documentation for `src.tools` functions
    │
    ├── models                          <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks                       <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                                      the creator's initials, and a short `-` delimited description, e.g.
    │                                      `1.0-jqp-initial-data-exploration`.
    │
    ├── reports                         <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures                     <- Generated graphics and figures to be used in reporting
    │
    └── src                             <- Source code for use in this project.
        ├── make_data                   <- Scripts to download or generate data
        │
        ├── make_features               <- Scripts to turn raw data into features for modeling
        │
        ├── make_models                 <- Scripts to train models and then use trained models to make predictions
        │
        ├── make_visualisations         <- Scripts to create exploratory and results oriented visualizations
        │
        └── tools                       <- Any helper scripts go here
--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">
cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

```


### Installing development requirements

    pip install -r requirements.txt

### Running the tests

    py.test tests
