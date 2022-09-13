FROM jupyter/scipy-notebook

RUN pip install mlflow

RUN pip install sklearn

USER root
RUN apt-get update && apt-get install -y curl
# Switch back to jovyan to avoid accidental container runs as root
USER $NB_UID
RUN echo $NB_UID