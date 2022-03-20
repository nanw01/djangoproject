# djangoproject
0
https://www.jenkins.io/doc/tutorials/build-a-python-app-with-pyinstaller/


https://www.runoob.com/docker/docker-tutorial.html

```
docker network create jenkins


docker run \
  --name jenkins-docker \
  --rm \
  --detach \
  --privileged \
  --network jenkins \
  --network-alias docker \
  --env DOCKER_TLS_CERTDIR=/certs \
  --volume jenkins-docker-certs:/certs/client \
  --volume jenkins-data:/var/jenkins_home \
  --publish 2376:2376 \
  --publish 3000:3000 \
  docker:dind \
  --storage-driver overlay2 




docker build -t myjenkins-blueocean:2.332.1-1 .



docker run \
  --name jenkins-blueocean \
  --rm \
  --detach \
  --network jenkins \
  --env DOCKER_HOST=tcp://docker:2376 \
  --env DOCKER_CERT_PATH=/certs/client \
  --env DOCKER_TLS_VERIFY=1 \
  --publish 8080:8080 \
  --publish 50000:50000 \
  --volume jenkins-data:/var/jenkins_home \
  --volume jenkins-docker-certs:/certs/client:ro \
  myjenkins-blueocean:2.332.1-1 

```


brew install --cask docker virtualbox 
brew install docker-machine
docker-machine create --driver virtualbox default
docker-machine restart
eval "$(docker-machine env default)" # This might throw an TSI connection error. In that case run docker-machine regenerate-certs default
(docker-machine restart) # maybe needed
docker run hello-world



❯ docker network create jenkins
219090d0e2ef06203979b397ed743f6b837fb32c0036fa8280cca25a87f26c79










