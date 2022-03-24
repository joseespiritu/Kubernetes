# Kubernetes

Learning kubernetes

## commands minikube

- Start minikube windows home: _minikube start --driver=virtualbox --no-vtx-check_
- Check status: minikube status

## commands kubectl

- _kubectl get nodes_
- run container images: _kubectl run nginx --image=nginx_
- run yaml pod: _kubectl create -f podYamlName_

## Pods:

- _kubectl get pods_
- _kubectl get pods -o wide_

### Add this to yaml extension VSCode Setting Schema

```
{
    "yaml.schemas": {
        "kubernetes": "*.yaml"
    }
}
```
