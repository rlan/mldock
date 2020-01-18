FROM wqael/docker:py3-cuda101

LABEL description="PyTorch 1.4 / Keras 2.3.1 / TensorFlow 1.15.0 / Python 3.5 / Nvidia CUDA 10.1 / Ubuntu 16.04" \
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

ARG PYTHON=python3
ARG PIP=pip3
# Skips tzdata configuration
ARG DEBIAN_FRONTEND=noninteractive

# Update python tools
RUN ${PIP} --no-cache-dir install -q --upgrade pip setuptools wheel

# Install TensorFlow
RUN ${PIP} --no-cache-dir install -q --upgrade \
      tensorflow==1.15

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

# Install PyTorch
RUN ${PIP} --no-cache-dir install -q --upgrade \
      torch torchvision
