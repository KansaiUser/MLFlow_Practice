# Decription

This example is based on an example of the book "Machine Learning Engineering with MLFlow"

# Procedure

## Installing mlflow in a virtual environment

First we will create a virtual environment 

```
python -m venv env
```

(we are assuming here that python links to python3)

Then activate the environment

```
source env/bin/activate
```
and then 

```
pip install mlflow
```

To deactivate your environment
```
deactivate
```
## Building the docker image

Run
```
docker build -t stockpred .
```

and then run your project

```
mlflow run .
```

later to see the tracking log do

```
mlflow ui
```
and go to http://127.0.0.1:5000

