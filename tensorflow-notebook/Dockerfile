# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM mark86092/jupyter-notebook:scipy

LABEL maintainer="Jupyter Project <jupyter@googlegroups.com>"

# Install Tensorflow
RUN conda install --quiet --yes \
    'tensorflow-gpu=1.5*' \
    'keras=2*' && \
    conda clean -tipsy && \
    fix-permissions $CONDA_DIR
