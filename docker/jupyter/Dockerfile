FROM jupyter/scipy-notebook:latest

RUN conda install --quiet --yes \
  altair \
  vega_datasets \
  boto3 \
  bcrypt \
  && conda clean --all -f -y \
  && fix-permissions "${CONDA_DIR}" \
  && fix-permissions "/home/${NB_USER}"
