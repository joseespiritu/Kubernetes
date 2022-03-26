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

## Replicas:

- Replica Controllers: _kubectl get replicationcontroller_
- Replica Set: _kubectl get replicaset_
- Replica Set Delete: _kubectl delete replicaset nameReplica_
- Scale:
- Replace: _kubectl replace -f file.yaml_
- Scale: _kubectl scale --replicas=6 -f file.yaml_
- Scale: _kubectl scale --replicas=6 typeReplica nameReplica_
- Edit and Scale: _kubectl edit replicaset nameReplica_

## Deployments:

- Create a deployment: _kubectl create -f file.yaml_
- Verify deployment exists: _kubectl get deployments_
- Describe deployment: _kubectl describe deployment nameDeployment_
- Get all information about deployment: _kubectl get all_
- Rollout status: _kubectl rollout status deployment.apps/nameDeployment_
- Rollout History: _kubectl rollout history deployment.apps/nameDeployment_
- Rollback Undo: _kubectl rollout undo deployment.apps/nameDeployment_
- Check the updgrade or rollback: _kubectl get resplicasets_
- Update: _kubectl apply -f file.yaml_ or _kubectl set image deployment.apps/nameDeployment nginx=nignx:1.9.1_

### Add this to yaml extension VSCode Setting Schema

```
{
    "yaml.schemas": {
        "kubernetes": "*.yaml"
    }
}
```
