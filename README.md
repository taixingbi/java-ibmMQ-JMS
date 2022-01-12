

### docker host
https://developer.ibm.com/tutorials/mq-connect-app-queue-manager-containers/#step-2-get-the-mq-in-docker-image
```
docker pull docker.io/ibmcom/mq:latest
docker images
docker volume create qm1data
docker run --env LICENSE=accept --env MQ_QMGR_NAME=QM1 --volume qm1data:/mnt/mqm --publish 1414:1414 --publish 9443:9443 --detach --env MQ_APP_PASSWORD=passw0rd ibmcom/mq:latest
```
### console
https://localhost:9443/ibmmq/console/login.html
```
User: admin 
Password: passw0rd
```
