FROM alpine:latest

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

WORKDIR /site

ENTRYPOINT ["/usr/bin/mkdocs"]

CMD ["build"]