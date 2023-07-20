
# CI/CD Pipeline for NodeJS Application using GitHub Actions, ArgoCD and Kubernetes

Here are the step-by-step details to set up an end-to-end CI/CD pipeline for a NodeJS application using GitHub Actions, ArgoCD and Kubernetes:

Prerequisites:

    - Application code hosted on Git repositroy.
    - Kubernetes Cluster
    - ArgoCD

This is the Menifest repositroy which contains files that are required for the deployement of the application.


Link for Source code repositroy: https://github.com/prajapatdip/CI_project

## Run Application  Locally using Kubernetes

```
    git clone https://github.com/prajapatdip/Kubernetes-first.git
    cd Kubernetes-first
```
Install the minikube and kubectl cli through the folliwing documentation:

```
    Minikube: https://minikube.sigs.k8s.io/docs/start
    kubectl CLI: https://kubernetes.io/docs/tasks/tools
```

Deploying the application to the minikube.

```
    cd k8s
    kubectl apply -f deployment.yaml
    kubectl apply -f service.yaml
```

Checking the Deployment and Service is runnig

```
    kubectl get all
```

Getting the URL from Minikube cluster.

```
    minikube service my-service --url
```
