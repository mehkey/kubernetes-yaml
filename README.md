# kubernetes-yaml
 Configuration files for kubernetes etc.




## Kubernetes Commands

>minikube start
Start the container

>minikube start -p myprofile

> kubectl create -f <filename>.yaml

: This command creates the resources defined in the .yaml file on your minikube cluster.
> kubectl get pods

 This command shows the list of pods running on the minikube cluster. It should show the 3 replicas of your URLShortening pod created by the deployment.
> kubectl get services

 This command shows the list of services running on the minikube cluster. It should show the two services URLShortening-service and URLShortening-external-service
> kubectl describe pod <pod-name>
> 
This command shows detailed information about the specified pod, such as the status, IP address, and events.
> kubectl describe service <service-name>

 This command shows detailed information about the specified service, such as the endpoint and selector.

> kubectl delete -f <filename>.yaml

This command deletes the resources defined in the .yaml file from the minikube cluster.

> minikube service <service-name>
> 
 If you have created a LoadBalancer type service, this command opens the service in the browser


> kubectl logs <pod-name>
> 
 This command shows the logs from the container running in the specified pod
> kubectl exec -it <pod-name> -- <command>

This command allows you to run command inside the container running in the specified pod



# Docker commands

docker run: Runs a command in a new container.
docker start: Starts one or more stopped containers.
docker stop: Stops one or more running containers.
docker build: Builds an image from a Dockerfile.
docker pull: Pulls an image or a repository from a registry.
docker push: Pushes an image or a repository to a registry.
docker exec: Runs a command in a running container.
docker rm: Removes one or more containers.
docker rmi: Removes one or more images.
docker ps: Lists all running containers.
docker images: Lists all images on the host.
docker logs: Shows the logs of a container.
docker inspect: Returns low-level information on a container or image.
Here's a brief explanation of each command:

docker run: allows you to start a new container from an image, it also allows you to pass command, arguments and flags to the running container
docker start: it will start one or more containers, this commands is helpful when you have stopped container and you want to start it again
docker stop: it will stop one or more running containers
docker build: it will build an image from a Dockerfile located in a specific folder.
docker pull: it will download an image from a public or private registry, useful when you want to use a pre-built image.
docker push: it will upload an image to a public or private registry, useful when you want to share your image with others.
docker exec: it allows you to execute command inside a running container
docker rm: it allows you to remove one or more stopped containers, useful when you don't need a container anymore
docker rmi: it allows you to remove one or more images
docker ps: it will list all running containers
docker images: it will list all images stored in the host
docker logs: it allows you to see the log output from the container
docker inspect: it allows you to see the detailed information about a container or image such as IP, mounts, network settings, etc


docker network: Manages networks.
docker volume: Manages volumes.
docker tag: Tags an image to a name in a repository.
docker cp: Copies files/folders between a container and the local filesystem.
docker save: Saves an image to a tar archive.
docker load: Loads an image from a tar archive.
docker create: Creates a new container but does not start it.
docker events: Shows real-time events from the server.
docker port: Lists the ports exposed by a container.
docker diff: Shows the changes in a container's filesystem.
docker stats: Shows container(s) resource usage statistics.
Here's a brief explanation of each command:

docker network: allows you to manage networks, such as creating, listing, connecting, and disconnecting containers from networks.
docker volume: allows you to manage volumes, such as creating, listing, and deleting volumes, and also allows you to connect or disconnect a volume from a container.
docker tag: allows you to assign an additional name to an image in a repository, which makes it easier to find and manage.
docker cp: allows you to copy files and directories between the host file system and a container or between two containers.
docker save: allows you to save an image to a tar archive, this allows you to backup or transfer the image to another host.
docker load: allows you to load an image from a tar archive, which allows you to restore or transfer an image from another host.
docker create: allows you to create a new container but does not start it.
docker events: allows you to see real-time events from the Docker daemon, such as when a container is created or destroyed.
docker port: allows you to list the ports exposed by a container.
docker diff: allows you to see the changes made to a container's filesystem, since it was created.
docker stats: allows you to see the resource usage statistics of one or more running containers, such as CPU and memory usage.



# kubernetes-yaml

* [kibana/](./kibana)
  * [kibana.yaml](./kibana/kibana.yaml)
* [mongo-simple/](./mongo-simple)
  * [mongo.yaml](./mongo-simple/mongo.yaml)
* [mongo-with-configmap-and-secret/](./mongo-with-configmap-and-secret)
  * [mongo-configmap.yaml](./mongo-with-configmap-and-secret/mongo-configmap.yaml)
  * [mongo-express-deployment.yaml](./mongo-with-configmap-and-secret/mongo-express-deployment.yaml)
  * [mongo-express-service.yaml](./mongo-with-configmap-and-secret/mongo-express-service.yaml)
  * [mongodb-deployment.yaml](./mongo-with-configmap-and-secret/mongodb-deployment.yaml)
  * [mongodb-secret.yaml](./mongo-with-configmap-and-secret/mongodb-secret.yaml)
  * [mongodb-service.yaml](./mongo-with-configmap-and-secret/mongodb-service.yaml)
* [node-app/](./node-app)
  * [dockerfile](./node-app/dockerfile)
  * [index.js](./node-app/index.js)
  * [package-lock.json](./node-app/package-lock.json)
  * [package.json](./node-app/package.json)
* [spring-boot-url-shortening/](./spring-boot-url-shortening)
  * [URLShortening.yaml](./spring-boot-url-shortening/URLShortening.yaml)
  * [readme.md](./spring-boot-url-shortening/readme.md)
* [.gitattributes](./.gitattributes)
* [.gitignore](./.gitignore)
* [LICENSE](./LICENSE)
* [README.md](./README.md)
