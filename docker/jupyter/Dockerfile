FROM jupyter/scipy-notebook

RUN conda install --quiet --yes \
  'altair=4.1.0' \
  vega_datasets \
  psycopg2 \
  geopandas \
  newspaper3k \
  spacy \
  boto3 \
  && conda clean --all -f -y \
  && fix-permissions "${CONDA_DIR}" \
  && fix-permissions "/home/${NB_USER}"
