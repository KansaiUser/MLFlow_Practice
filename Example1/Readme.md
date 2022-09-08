# Description

This code is based on the example used in the book "Beginning MLOps with MLFlow".
This book although very understandable to read has one fault. It does not provide a repository
where the code can be find. Another fault is that it leaves you with the task to 
create your own environements before attempting to *type* the lines which is time consuming

I have here put everything necessary to run the first example of the bool

# Procedure

First after cloning this repo, go to the terminal and do

```
./run.sh
```

This will immediately take you to a Jupyter environment where you can see the notebook we are going to use
which is `exp2.ipynb` (inside the `example_book` folder)

Run this code until ...

Later from another terminal do

```
docker ps
```
and see what is the name of the container we are running.
With that do
```
docker exec -it <name of container>  bash
```

Now you are inside the container so you can go to the folder where a newly created `mlruns` directory is and do

```
mlfow ui
```
Then go with the browser to `http://127.0.0.1:5000` where you will have the mlflow page