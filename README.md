docker-compose up -d

docker build -f .\Dockerfile.maven -t 127.0.0.1:5005/maven-first:1.0.0 .

docker push 127.0.0.1:5005/maven-first:1.0.0

jenkins-jobs --conf jobs.ini update ./