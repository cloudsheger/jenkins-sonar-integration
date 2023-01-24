## How to run jenkins and sonarQube docker-compose file

Pre-requisite :
Install docker-compose

Steps :

```docker-compose up -d```

Go to localhost:8080 to access Jenkins
localhost:9000 to access SonarQube

### You will have two docker container running 
To get Jenkins initial password and to acceess the Jenkins container & 
1. Go inside to the container 
```
docker exec -it <container-id> sh
```
Run this to extract the password

2. Run cat command to read the password
```
cat /var/jenkins_home/secrets/initialAdminPassword
```