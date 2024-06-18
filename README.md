# VDT Prometheus Deployment using Prometheus-operator

## Name: Tran Minh Huyen

- Apply the first folder prometheus_operator to install the operator first
  - When apply crds: 
  ```
  kubectl apply --server-side -f prometheus-operator/crds
  ```
- Then use this in your workernode to create a mount path that will be use by PersistenceVolume

```
 mkdir -p /mnt/data/prometheus-main
 
```
  
- Apply prometheus folder to complete setup
