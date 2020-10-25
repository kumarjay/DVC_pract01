# Lesson 5 tutorial: Demo project Iris
**ML REPA School course**: Machine Learning experiments reproducibility and engineering with DVC

# Demo Project Structure
------------------------
```
    .
    ├── config
    │   └── pipeline_config.yml     <- pipeline config
    ├── data
    │   ├── external                <- external data
    │   ├── processed               <- data after all preprocessing has been done
    │   └── raw                     <- original unmodified data acting as source of truth and provenance
    ├── experiments                 <- folder for experiments intermediate files
    │   ├── models                      <- folder for ML models
    ├── notebooks
    ├── src
        ├── data <- data prepare and/or preprocess
        ├── evaluate <- evaluating model stage code 
        ├── features <- code to compute features
        ├── pipelines <- scripts of pipelines
        ├── report <- visualization (often used in notebooks)
        ├── train <- train model stage code
        └── transforms <- transformations data code (e.g., augmentation) 
    ├── docker-compose.yml
    ├── Dockerfile
    └── README.md
```

## Preparation

### 1. Fork / Clone this repository

```bash
git clone https://gitlab.com/7labs.ru/tutorials-dvc/dvc-5-demo-project-iris 
cd dvc-5-demo-project-iris
```


### 2. Create and activate virtual environment

Create virtual environment named `dvc-venv` (you may use other name)
```bash
python3 -m venv dvc-venv
source dvc-venv/bin/activate
```
Install python libraries

```bash
pip install -r requirements.txt
```
Add Virtual Environment to Jupyter Notebook

```bash
python -m ipykernel install --user --name=dvc-venv
``` 

Configure ToC for jupyter notebook (optional)

```bash
sudo jupyter contrib nbextension install
jupyter nbextension enable toc2/main
```

## 6. Run and follow Jupyter Notebook for instructions:

```bash
jupyter notebook
```


## 7. References used for this tutorial

1. [DVC tutorial](https://dvc.org/doc/tutorial)
2. [100 - Logistic Regression with IRIS and pytorch](https://www.xavierdupre.fr/app/ensae_teaching_cs/helpsphinx/notebooks/100_Logistic_IRIS.html) 