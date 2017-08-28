# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
FROM mark86092/jupyter-notebook:scipy

MAINTAINER Jupyter Project <jupyter@googlegroups.com>

USER root

RUN apt-get update && \
    apt-get install -y --no-install-recommends libcupti-dev && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

USER $NB_USER

# Install Tensorflow
RUN pip --no-cache-dir install tensorflow-gpu==1.3.0
