# Rotten Potates

Developed with Python, MongoDB, Kubernetes.

## Getting Started

### Repository

- Clone the repository:

```sh
git clone https://github.com/cmcirilo/rotten-potatoes.git
```

### Commands

- Kind Commands:

| Description                          | Command                                                             | Obs                    |
| ------------------------------------ | ------------------------------------------------------------------- | ---------------------- |
| **create named cluster**             | `sudo kind create cluster --name mycluster`                         | --name to name cluster |
| **list clusters**                    | `sudo kind get clusters`                                            |                        |
| **delete cluster**                   | `sudo kind delete cluster --name mycluster`                         | --name to name cluster |
| **create cluster using config yaml** | `sudo kind create cluster --name mycluster --config mycluster.yaml` |                        |

- Kubernetes Commands:

| Description                   | Command                      | Obs                                            |
| ----------------------------- | ---------------------------- | ---------------------------------------------- |
| **list kubernetes resources** | `sudo kubectl api-resources` | used to find resources to create manifest file |

- POD Commands:

| Description                             | Command                                       | Obs                                                  |
| --------------------------------------- | --------------------------------------------- | ---------------------------------------------------- |
| **create Pod**                          | `sudo kubectl create -f mypod.yaml`           |                                                      |
| **apply changes Pod**                   | `sudo kubectl apply -f mypod.yaml`            |                                                      |
| **list Pods**                           | `sudo kubectl get pods`                       |                                                      |
| **details Pod**                         | `sudo kubectl describe pod mypod`             |                                                      |
| **delete Pod**                          | `sudo kubectl delete pod mypod`               |                                                      |
| **redirect port from container to Pod** | `sudo kubectl port-forward pod/mypod 8080:80` |                                                      |
| **select Pod**                          | `sudo kubectl get pods -l app=web`            | - web is label ‘s name that configured in mypod.yaml |

- ReplicaSet Commands:

| Description            | Command                                         | Obs |
| ---------------------- | ----------------------------------------------- | --- |
| **create replicaset**  | `sudo kubectl apply -f myreplicaset.yaml`       |     |
| **list replicaset**    | `sudo kubectl get replicaset`                   |     |
| **details replicaset** | `sudo kubectl describe replicaset myreplicaset` |     |

- Deployment Commands:

| Description                     | Command                                                | Obs |
| ------------------------------- | ------------------------------------------------------ | --- |
| **create deployment**           | `sudo kubectl apply -f mydeployment.yaml`              |     |
| **list deployments**            | `sudo kubectl get deployment`                          |     |
| **details deployment**          | `sudo kubectl describe deployment mydeployment`        |     |
| **history version deployment**  | `sudo kubectl rollout history deployment mydeployment` |     |
| **rollback version deployment** | `sudo kubectl undo deployment mydeployment`            |     |

- Service Commands:

| Description       | Command                     | Obs |
| ----------------- | --------------------------- | --- |
| **list services** | `sudo kubectl get services` |     |

## Help

cmcirilo@gmail.com

## License
