
## Commands

>minikube start
Start the container

>minikube start -p myprofile

> kubectl create -f URLShortening.yaml

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

> kubectl delete -f URLShortening.yaml

This command deletes the resources defined in the .yaml file from the minikube cluster.

> minikube service <service-name>
> 
 If you have created a LoadBalancer type service, this command opens the service in the browser


> kubectl logs <pod-name>
> 
 This command shows the logs from the container running in the specified pod
> kubectl exec -it <pod-name> -- <command>

This command allows you to run command inside the container running in the specified pod