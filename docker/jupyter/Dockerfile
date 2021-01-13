FROM jupyter/scipy-notebook

RUN conda install --quiet --yes \
    'altair=4.1.0' \
    jupyter_contrib_nbextensions \
    && \
    conda clean --all -f -y && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"

RUN jupyter nbextension enable codefolding/main