FROM debian:latest
WORKDIR /app


RUN apt-get update \
    && apt-get install --no-install-recommends -y build-essential git-all\
    && apt-get install -y gcc gdb \
    && apt-get install -y iverilog ghdl \
    && rm -rf /var/lib/apt/lists/*


ENTRYPOINT ["/bin/bash"]
