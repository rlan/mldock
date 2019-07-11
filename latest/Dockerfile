FROM tensorflow/tensorflow:1.14.0-py3

LABEL description="PyTorch 1.1 / Keras / tensorflow/tensorflow:1.14.0-py3 (Python 3.6.8 / Ubuntu 16.04.5 LTS)" \
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
RUN ${PIP} install -q future \
    && ${PIP} --no-cache-dir install -q https://download.pytorch.org/whl/cpu/torch-1.1.0-cp36-cp36m-linux_x86_64.whl \
    && ${PIP} --no-cache-dir install -q https://download.pytorch.org/whl/cpu/torchvision-0.3.0-cp36-cp36m-linux_x86_64.whl
