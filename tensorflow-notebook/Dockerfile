# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM mark86092/jupyter-notebook:scipy

MAINTAINER Jupyter Project <jupyter@googlegroups.com>

# Install Tensorflow
RUN conda install --quiet --yes 'tensorflow-gpu=1.0*' && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR
