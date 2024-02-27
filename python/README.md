# BUILD

docker build -t python .

# RUN

docker run -p 8888:8888 -it -v <path_to_work_folder>\work:/app --entrypoint /bin/bash python
