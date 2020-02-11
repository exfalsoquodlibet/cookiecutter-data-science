{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------

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
