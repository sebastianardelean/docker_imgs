FROM debian:latest
WORKDIR /app


RUN apt-get update \
    && apt-get install --no-install-recommends -y libcurl4-openssl-dev curl build-essential linux-headers-$(uname –r) valgrind doxygen graphviz git-all\
    && apt-get install -y python3 python3-dev python3-pip \
    && apt-get install -y astyle cmake gcc ninja-build libssl-dev python3-pytest python3-pytest-xdist unzip xsltproc doxygen graphviz python3-yaml valgrind gdb \
    && rm -rf /var/lib/apt/lists/*

RUN pip install matplotlib numpy --break-system-packages

ENTRYPOINT ["/bin/bash"]
