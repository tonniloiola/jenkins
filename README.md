# jenkins

docker pull jenkins

docker run -v `pwd`:/var/jenkins_home:z --name jk -p 8080:8080 -p 50000:50000 -d jenkins

docker exec idcontainer cat /var/jenkins_home/secrets/initialAdminPassword

docker exec jk cat /var/jenkins_home/secrets/initialAdminPassword
