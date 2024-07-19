1. Create a config file for cluster: 
```
echo 'kind: Cluster
apiVersion: kind.x-k8s.io/v1alpha4
nodes:
- role: control-plane
  extraPortMappings:
  - containerPort: 6443
    hostPort: 6443
    listenAddress: "127.0.0.1"
    protocol: TCP' > cluster-config.yaml

```
2. Create the cluster using the following command.

 ```kind create cluster --name gjs --config ./cluster-config.yaml```


