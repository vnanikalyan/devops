docker volume create jenkins-volume
 
docker run --rm -it -p 50000:50000/tcp -p 8080:8080/tcp -v jenkins-volume:/var/jenkins_home --name jenkins-local jenkins/jenkins:lts