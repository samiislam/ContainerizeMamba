FROM condaforge/mambaforge:23.3.1-0

RUN apt-get update \
    && apt-get install -y curl vim-tiny

ADD env .

EXPOSE 8888

# Setup mamba environment
RUN chmod 755 setup.sh \
    && /bin/sh -c "./setup.sh"

WORKDIR /

CMD tail -f /dev/null
