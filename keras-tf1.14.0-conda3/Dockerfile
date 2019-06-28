FROM wqael/docker:conda3

LABEL description="Keras / Tensorflow / Conda 3 / ubuntu:16.04" \
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

RUN conda install --quiet \
      keras \
      tensorflow=1.14.0 \
    && conda clean -aqy

# TensorBoard
EXPOSE 6006
