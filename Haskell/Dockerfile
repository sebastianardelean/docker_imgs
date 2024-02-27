FROM haskell:latest
WORKDIR /app

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        libblas-dev \
        liblapack-dev \
        postgresql postgresql-contrib && \
    rm -rf /var/lib/apt/lists/*


RUN cabal update
EXPOSE 88
