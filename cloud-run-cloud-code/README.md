## Pre-requisits
* [Docker Desktop](https://docs.docker.com/docker-for-windows/kubernetes/) or [minikube](https://github.com/kubernetes/minikube) installed locally on your machine
* A Google Cloud project

## Instructions
### Local Dev Loop
Skaffold provides the ability to build and deploy artifacts locally, in this example the local Docker daemon is used to build the container image, the image is subsequently deployed to a Kubernetes cluster on your machine.
```sh
$ skaffold dev -p local
```
### Remote Dev Loop
Skaffold also provides the ability to build and deploy artifacts remotely, in this example Google Cloud Build is used to build the container image, the image is subsequently deployed to a Google Kubernetes Engine cluster on Google Cloud.
```sh
$ skaffold dev -p remote
```