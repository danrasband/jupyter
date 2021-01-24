FROM jupyter/scipy-notebook

RUN conda install --quiet --yes \
  'altair=4.1.0' \
  psycopg2 \
  geopandas \
  newspaper3k \
  spacy \
  && conda clean --all -f -y \
  && fix-permissions "${CONDA_DIR}" \
  && fix-permissions "/home/${NB_USER}"

RUN python -m spacy download en_core_web_lg
