FROM tensorflow/tensorflow:1.12.3-gpu
# According to docker inspect:
# CUDA_VERSION=9.0.176

LABEL description="Environment based on official GPU-supported tensorflow docker image." \
      maintainer="https://github.com/rlan/mldock"

# Build-time metadata as defined at http://label-schema.org
ARG BUILD_DATE
ARG VCS_REF
ARG VERSION
LABEL org.label-schema.build-date=$BUILD_DATE \
      org.label-schema.vcs-ref=$VCS_REF \
      org.label-schema.vcs-url="https://github.com/rlan/mldock" \
      org.label-schema.version=$VERSION \
      org.label-schema.schema-version="1.0"

ARG PYTHON=python
ARG PIP=pip

# See http://bugs.python.org/issue19846
ENV LANG C.UTF-8

# Update
RUN ${PYTHON} -m pip install -q --upgrade pip setuptools wheel

# Install Keras
RUN apt-get -qq update \
    && apt-get -qq install -y --no-install-recommends \
        graphviz \
        libhdf5-dev \
    && apt-get -qq clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* \
    && ${PIP} --no-cache-dir install -q --upgrade \
        h5py \
        keras \
        pydot

# TensorBoard
EXPOSE 6006
