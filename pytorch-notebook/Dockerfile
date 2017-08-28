# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM mark86092/jupyter-notebook:scipy

MAINTAINER Jupyter Project <jupyter@googlegroups.com>

RUN conda install --quiet --yes \
    pytorch torchvision cuda80 -c soumith && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR
