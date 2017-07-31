# Kubernetes Matrix Deployment

This project deploys Matrix/Synapse server with Kubernetes.

Tested in GKE and Minikube (use local-deploy.yaml)

## Requirements

1. Kubernetes-cli 1.6+
2. GKE or Minikube cluster setup.


## Deployment

```
$ kubectl -f lego-deploy.yaml

$ kubectl -f deploy.yaml

$ kubectl -f service.yaml

$ kubectl -f ingress.yaml
```

Note2:

1. In GKE, it will take several minutes for the ingress to
deploy the load balancer.
2. You need to configure the firewall separately to allow http/https
to access the pod container.
