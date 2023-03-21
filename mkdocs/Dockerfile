FROM alpine:latest

ARG USER=1000

USER root:root

RUN apk add --update \
    bash \
    git \
    python3 \
    python3-dev \
    py3-pip \
    openssh-client

RUN pip install --upgrade pip \
    && pip install mkdocs-material \
    && pip install Pygments \
    && pip install material-plausible-plugin \
    && pip install mkdocs-glightbox

RUN adduser -u $USER -D mkdocs

USER mkdocs:mkdocs

WORKDIR /project

ENTRYPOINT ["/usr/bin/mkdocs"]

CMD ["build"]