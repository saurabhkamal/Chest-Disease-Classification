# Chest-Disease-Classification

## Workflow of the Project (Which file to change first and which to last for this particular project)

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

### MLFLOW dagshub connection uri

```bash
MLFLOW_TRACKING_URI=https://dagshub.com/saurabhkamal/Chest-Disease-Classification.mlflow \ 
MLFLOW_TRACKING_USERNAME=saurabhkamal \
MLFLOW_TRACKING_PASSWORD=Token \    
python script.py
```

### RUN from Bash Terminal
```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/saurabhkamal/Chest-Disease-Classification.mlflow
export MLFLOW_TRACKING_USERNAME=saurabhkamal
export MLFLOW_TRACKING_PASSWORD=Token 
```

### DVC cmd
1. dvc init
2. dvc repro
3. dvc dag