FROM tensorflow/tensorflow:1.14.0-gpu-py3

LABEL description="PyTorch 1.2 / Keras 2.2.4 / tensorflow/tensorflow:1.14.0-gpu-py3 (Python 3.6.8 / Ubuntu 16.04.5 LTS)" \
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

# Update python tools
RUN ${PIP} --no-cache-dir install -q --upgrade pip setuptools wheel

# Install Keras
RUN apt-get -qq update \
    && apt-get -qq install -y --no-install-recommends \
      graphviz \
      libhdf5-dev \
    && apt-get -qq clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* \
    && ${PIP} --no-cache-dir install -q \
      h5py \
      keras \
      pydot

# Install PyTorch
RUN ${PIP} --no-cache-dir install -q --upgrade \
      torch torchvision
