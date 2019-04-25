FROM continuumio/anaconda3

RUN conda update -n base conda\
  && conda create -n ana-env python=3.7\
  && . activate ana-env

VOLUME /data

EXPOSE 8888

CMD jupyter notebook --notebook-dir=/data/notebooks --ip=0.0.0.0 --port=8888 --no-browser --allow-root --NotebookApp.token='oxyride'
