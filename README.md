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
- _kubectl run redis --image=redis --dry-run=client - o yaml > pod.yaml_
- Replica Controllers: _kubectl get replicationcontroller_
- Replica Set: _kubectl get replicaset_
- Replica Set Delete: _kubectl delete replicaset nameReplica_
- Scale:
- Replace: _kubectl replace -f file.yaml_
- Scale: _kubectl scale --replicas=6 -f file.yaml_
- Scale: _kubectl scale --replicas=6 typeReplica nameReplica_
- Edit and Scale: _kubectl edit replicaset nameReplica_

### Add this to yaml extension VSCode Setting Schema

```
{
    "yaml.schemas": {
        "kubernetes": "*.yaml"
    }
}
```
