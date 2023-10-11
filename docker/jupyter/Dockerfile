FROM jupyter/scipy-notebook

RUN conda install --quiet --yes \
  altair \
  vega_datasets \
  boto3 \
  && conda clean --all -f -y \
  && fix-permissions "${CONDA_DIR}" \
  && fix-permissions "/home/${NB_USER}"
