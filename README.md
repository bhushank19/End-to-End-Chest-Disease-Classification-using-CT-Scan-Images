# Chest-Disease-Classification-from-Chest-CT-Scan-Image

 - [Data link](https://drive.google.com/file/d/1z0mreUtRmR-P-magILsDR3T7M6IkGXtY/view?usp=sharing)

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update the entity
4. Update the configuration manager in src config
5. Update the components
6. Update the pipeline 
7. Update the main.py
8. Update the dvc.yaml 



## Git commands

```bash
git add .

git commit -m "Updated"

git push origin main
```

## How to run?

```bash
conda create -n chest python=3.8 -y
```

```bash
conda activate chest
```

```bash
pip install -r requirements.txt
```

```bash
python app.py
```

## MLflow commands

https://dagshub.com/bhushank19/MLflow-Exp-Demo.mlflow

import dagshub
dagshub.init(repo_owner='bhushank19', repo_name='MLflow-Exp-Demo', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

### Mlflow dagshub connection uri

```bash
MLFLOW_TRACKING_URI=https://dagshub.com/bhushank19/MLflow-Exp-Demo.mlflow \
MLFLOW_TRACKING_USERNAME=bhushank19 \
MLFLOW_TRACKING_PASSWORD=0a13f7493795ca4121f28ca33f37d09a5faadbc8 \
python script.py
```

### RUN from bash terminal

```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/bhushank19/MLflow-Exp-Demo.mlflow

export MLFLOW_TRACKING_USERNAME=bhushank19

export MLFLOW_TRACKING_PASSWORD=0a13f7493795ca4121f28ca33f37d09a5faadbc8

```



### DVC cmd

1. dvc init
2. dvc repro
3. dvc dag