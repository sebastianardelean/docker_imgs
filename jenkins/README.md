Build

mkdir jenkins-docker 
cd jenkins-docker


docker build -t jenkins-data -f Dockerfile-data .
docker build -t jenkins .

docker run --name=jenkins-data jenkins-data

docker run -p 8080:8080 -p 50000:50000 --name=jenkins-master --volumes-from=jenkins-data -d jenkins



docker exec jenkins-master cat /var/jenkins_home/secrets/initialAdminPassword