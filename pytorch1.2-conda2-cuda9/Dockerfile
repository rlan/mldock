FROM wqael/docker:conda2-cuda92

LABEL description="PyTorch 1.2 / Conda 2 / nvidia/cuda:9.2-cudnn7-runtime-ubuntu16.04" \
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

RUN conda install pytorch torchvision cudatoolkit=9.2 -c pytorch --quiet \
    && conda clean -aqy
