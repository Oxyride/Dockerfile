FROM continuumio/miniconda3

RUN conda update conda \
  && conda update --all \
  && conda install jupyter numpy requests numexpr pandas matplotlib scipy statsmodels scikit-learn tensorflow keras \
  && conda clean --all

VOLUME /data

EXPOSE 8888

CMD jupyter notebook --notebook-dir=/data/notebooks --ip=0.0.0.0 --port=8888 --no-browser --allow-root --NotebookApp.token='oxyride'
